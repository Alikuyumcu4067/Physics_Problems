## 9. Damped Oscillator Simulation

**Problem:**
A damped harmonic oscillator is governed by the differential equation:
$$m \frac{d^2x}{dt^2} + b \frac{dx}{dt} + kx = 0$$
where $m = 1 \text{ kg}$, $k = 5 \text{ N/m}$, and $b$ is the damping coefficient.
1. Solve for the position $x(t)$ given $x(0) = 1$ and $v(0) = 0$.
2. Create an interactive simulation to visualize the effect of damping.

**Solution:**
The system's behavior is determined by the damping constant $b$. The roots of the characteristic equation provide three distinct cases:
* **Underdamped ($b^2 < 4mk$):** The system oscillates with an exponentially decaying amplitude.
* **Critically Damped ($b^2 = 4mk$):** The system returns to equilibrium in the shortest time without oscillation.
* **Overdamped ($b^2 > 4mk$):** The system returns to equilibrium slowly without any oscillation.

### Interactive Simulation Code
Copy the code below into an `.html` file to run the simulation in a web browser:

```html
<!DOCTYPE html>
<html>
<head>
    <title>Damped Oscillator Simulation</title>
    <script src="[https://cdn.plot.ly/plotly-latest.min.js](https://cdn.plot.ly/plotly-latest.min.js)"></script>
    <style>
        body { font-family: Arial, sans-serif; text-align: center; background: #fdfdfd; }
        #controls { margin: 20px; padding: 15px; background: #eee; border-radius: 10px; display: inline-block; }
    </style>
</head>
<body>
    <h1>Damped Harmonic Motion</h1>
    <div id="controls">
        <label>Damping Coefficient (b): </label>
        <input type="range" id="b_val" min="0" max="10" step="0.1" value="0.5">
        <span id="b_display">0.5</span>
    </div>
    <div id="plot" style="width:95%; height:500px; margin:auto;"></div>

    <script>
        const m = 1, k = 5;
        const bSlider = document.getElementById('b_val');
        const bDisplay = document.getElementById('b_display');

        function updatePlot() {
            let b = parseFloat(bSlider.value);
            bDisplay.innerText = b;

            let x = 1, v = 0, t = 0, dt = 0.04;
            let timeArr = [], posArr = [];

            // RK4 Numerical Integration
            const accel = (x, v, b) => -(b * v + k * x) / m;

            for (let i = 0; i < 600; i++) {
                timeArr.push(t.toFixed(2));
                posArr.push(x);

                let k1v = accel(x, v, b), k1x = v;
                let k2v = accel(x + 0.5 * dt * k1x, v + 0.5 * dt * k1v, b), k2x = v + 0.5 * dt * k1v;
                let k3v = accel(x + 0.5 * dt * k2x, v + 0.5 * dt * k2v, b), k3x = v + 0.5 * dt * k2v;
                let k4v = accel(x + dt * k3x, v + dt * k3v, b), k4x = v + dt * k3v;

                v += (dt / 6) * (k1v + 2 * k2v + 2 * k3v + k4v);
                x += (dt / 6) * (k1x + 2 * k2x + 2 * k3x + k4x);
                t += dt;
            }

            Plotly.newPlot('plot', [{
                x: timeArr, y: posArr, mode: 'lines', line: {color: '#d62728', width: 3}
            }], {
                title: 'Displacement x(t) over Time',
                xaxis: { title: 'Time (s)' },
                yaxis: { title: 'Position (m)', range: [-1.2, 1.2] }
            });
        }

        bSlider.oninput = updatePlot;
        updatePlot();
    </script>
</body>
</html>
