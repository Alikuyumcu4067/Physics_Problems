# Question 8: Mass-Spring System Simulation, Metrology, and Quantitative Uncertainty Analysis

## 1. Objective and Theoretical Framework
The objective of this laboratory exercise is to determine the spring constant ($k$) of a vertical Hookean harmonic oscillator and evaluate its experimental absolute uncertainty ($\delta k$). 

An ideal mass suspended on a vertical spring undergoes simple harmonic motion. The theoretical period ($T$) of a single complete oscillation is governed by the relation:
$$T = 2\pi\sqrt{\frac{m}{k}}$$

By isolating the spring constant ($k$), we derive the analytical physics model:
$$k = \frac{4\pi^2 m}{T^2}$$

### Metrological Constraints:
* The suspended mass is an exact benchmark standard: $m = 0.5000 \text{ kg}$ with zero uncertainty ($\delta m = 0$).
* To mitigate human reflex errors during manual stopwatch triggering, we measure the time taken for 10 complete oscillations ($t_{10}$) in each trial instead of a single cycle. The individual period for any trial is computed as:
  $$T_i = \frac{t_{10,i}}{10}$$

---

## 2. Interactive Simulator Source Code (HTML/JavaScript)

To perform this experiment digitally, save the following single-file code block with an `.html` extension (e.g., `spring_lab.html`) and execute it in a standard web browser. This simulation mimics an ideal spring system ($k = 20 \text{ N/m}$, $m = 0.5 \text{ kg}$) yielding a theoretical 10-cycle duration of approximately $9.93 \text{ seconds}$.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Mass-Spring Metrology Lab</title>
    <style>
        body { font-family: sans-serif; background: #f8fafc; color: #334155; padding: 20px; }
        .lab-card { background: white; max-width: 500px; margin: 0 auto; border: 1px solid #e2e8f0; border-radius: 8px; padding: 20px; box-shadow: 0 4px 6px rgba(0,0,0,0.05); }
        canvas { display: block; margin: 10px auto; background: #1e293b; border-radius: 4px; }
        .display { text-align: center; font-size: 2rem; font-family: monospace; margin: 10px 0; background: #f1f5f9; padding: 5px; border-radius: 4px; }
        .controls { display: flex; gap: 10px; justify-content: center; }
        button { padding: 10px 15px; font-weight: bold; border-radius: 4px; border: none; cursor: pointer; }
        .start { background: #16a34a; color: white; }
        .stop { background: #dc2626; color: white; }
        .reset { background: #475569; color: white; }
        .calc { background: #2563eb; color: white; width: 100%; margin-top: 15px; }
        .table-wrap { max-height: 200px; overflow-y: auto; margin-top: 15px; border: 1px solid #e2e8f0; }
        table { width: 100%; border-collapse: collapse; }
        th, td { padding: 6px; border-bottom: 1px solid #e2e8f0; text-align: center; font-size: 0.85rem; }
        th { background: #f1f5f9; }
        .output { margin-top: 15px; padding: 12px; background: #f0fdf4; border: 1px solid #bbf7d0; border-radius: 6px; color: #166534; display: none; font-family: monospace; }
    </style>
</head>
<body>
<div class="lab-card">
    <h3>Vertical Mass-Spring Oscillator Simulator</h3>
    <p style="font-size:0.8rem; color:#64748b;">Parameters: m = 0.5000 kg (Fixed). Measure 10 full cycles per trial.</p>
    <canvas id="canvas" width="160" height="180"></canvas>
    <div class="display" id="stopwatch">00:00.00</div>
    <div class="controls">
        <button class="start" id="actionBtn" onclick="toggleTimer()">Start</button>
        <button class="reset" onclick="resetTimer()">Reset</button>
    </div>
    <div class="table-wrap">
        <table>
            <thead><tr><th>Trial (i)</th><th>Time for 10 Cycles (t10, s)</th></tr></thead>
            <tbody id="tableBody"></tbody>
        </table>
    </div>
    <button class="calc" onclick="processLabData()">Run Metrological Reduction</button>
    <div class="output" id="labOutput"></div>
</div>
<script>
    let y=90, v=0, start=0, elapsed=0, tID=null;
    const canvas=document.getElementById('canvas'), ctx=canvas.getContext('2d');
    const tbody=document.getElementById('tableBody');
    for(let i=1; i<=10; i++) {
        tbody.innerHTML += `<tr><td>Trial ${i}</td><td><input type="number" step="0.01" class="lab-in" style="width:90%"></td></tr>`;
    }
    function fmt(ms) {
        let s=Math.floor(ms/1000), h=Math.floor((ms%1000)/10);
        return `${s.toString().padStart(2,'0')}.${h.toString().padStart(2,'0')} s`;
    }
    function toggleTimer() {
        const btn=document.getElementById('actionBtn');
        if(!tID) { start=Date.now()-elapsed; tID=setInterval(()=>{ elapsed=Date.now()-start; document.getElementById('stopwatch').innerText=fmt(elapsed); },10); btn.innerText="Stop"; btn.className="stop"; }
        else { clearInterval(tID); tID=null; btn.innerText="Start"; btn.className="start"; }
    }
    function resetTimer() { clearInterval(tID); tID=null; elapsed=0; document.getElementById('stopwatch').innerText="00:00.00 s"; document.getElementById('actionBtn').innerText="Start"; document.getElementById('actionBtn').className="start"; }
    function sim() {
        v += ((-20*(y-90))/0.5)*0.016; y += v*0.016;
        ctx.clearRect(0,0,160,180); ctx.strokeStyle="#94a3b8"; ctx.lineWidth=2; ctx.beginPath(); ctx.moveTo(80,0);
        for(let i=0; i<=10; i++) ctx.lineTo(i%2===0?70:90, (y/10)*i); ctx.stroke();
        ctx.beginPath(); ctx.arc(80,y,12,0,2*Math.PI); ctx.fillStyle="#38bdf8"; ctx.fill();
        requestAnimationFrame(sim);
    }
    function processLabData() {
        let ins=document.getElementsByClassName('lab-in'), periods=[];
        for(let i=0; i<ins.length; i++) {
            let val=parseFloat(ins[i].value); if(!isNaN(val)&&val>0) periods.push(val/10);
        }
        if(periods.length<2) { alert("Please input data for at least 2 trials."); return; }
        let n=periods.length, sum=periods.reduce((a,b)=>a+b,0), mean=sum/n;
        let sqSum=periods.reduce((a,b)=>a+Math.pow(b-mean,2),0), sd=Math.sqrt(sqSum/(n-1));
        let k=(4*Math.pow(Math.PI,2)*0.5)/Math.pow(mean,2), dk=k*2*(sd/mean);
        const out=document.getElementById('labOutput'); out.style.display="block";
        out.innerHTML=`<b>Processed Trials:</b> ${n}/10<br><b>Mean Period [T̄]:</b> ${mean.toFixed(4)} s<br><b>Std Dev [σ_T]:</b> ±${sd.toFixed(4)} s<br><b>Computed Spring Constant [k]:</b><br>k = (${k.toFixed(3)} ± ${dk.toFixed(3)}) N/m`;
    }
    sim();
</script>
</body>
</html>
