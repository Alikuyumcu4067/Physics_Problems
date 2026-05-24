# Question 7: Statistical Analysis of Test Scores (Mean and Standard Deviation)

## 1. Problem Statement
Eleven students received the following scores on an exam:
$$\text{Dataset: } \{88, 92, 79, 85, 95, 81, 86, 90, 83, 77, 89\}$$

Using a rigorous step-by-step method, calculate:
1. The sample mean ($\bar{x}$) and sample standard deviation ($\sigma$) for the **complete dataset** ($N = 11$).
2. The new sample mean and sample standard deviation after the **highest and lowest scores are removed** ($N = 9$).

### Mathematical Formulae:
* **Sample Mean:** $\bar{x} = \frac{1}{N} \sum_{i=1}^{N} x_i$
* **Sample Standard Deviation (Bessel's Correction):** $\sigma = \sqrt{\frac{1}{N-1} \sum_{i=1}^{N} (x_i - \bar{x})^2}$

---

## 2. Step-by-Step Solution: Complete Dataset ($N = 11$)

### Step 1: Calculate the Sum of All Scores
Sum all 11 data points in the sequence:
$$\sum x_i = 88 + 92 + 79 + 85 + 95 + 81 + 86 + 90 + 83 + 77 + 89 = 945$$

### Step 2: Calculate the Sample Mean ($\bar{x}$)
Divide the total sum by the number of samples ($N = 11$):
$$\bar{x} = \frac{945}{11} \approx 85.9091$$

### Step 3: Compute the Squared Deviations from the Mean $(x_i - \bar{x})^2$
Subtract the mean ($85.9091$) from each individual score, then square the result:

| $x_i$ | Deviation $(x_i - 85.9091)$ | Squared Deviation $(x_i - \bar{x})^2$ |
| :---: | :-------------------------: | :----------------------------------: |
| 88    | $+2.0909$                   | $4.3719$                             |
| 92    | $+6.0909$                   | $37.0991$                            |
| 79    | $-6.9091$                   | $47.7357$                            |
| 85    | $-0.9091$                   | $0.8265$                             |
| 95    | $+9.0909$                   | $82.6445$                            |
| 81    | $-4.9091$                   | $24.0993$                            |
| 86    | $+0.0909$                   | $0.0083$                             |
| 90    | $+4.0909$                   | $16.7355$                            |
| 83    | $-2.9091$                   | $8.4629$                             |
| 77    | $-8.9091$                   | $79.3721$                            |
| 89    | $+3.0909$                   | $9.5537$                             |
| **Sum**|                            | **$\sum (x_i - \bar{x})^2 = 310.9093$**|

### Step 4: Calculate the Variance and Sample Standard Deviation ($\sigma$)
Using Bessel's correction, divide the sum of squared deviations by $N - 1$ ($11 - 1 = 10$):
$$\text{Variance } (\sigma^2) = \frac{310.9093}{10} = 31.09093$$

Take the square root of the variance to determine the standard deviation:
$$\sigma = \sqrt{31.09093} \approx 5.5759$$

Rounding to two decimal places:
* **Mean ($\bar{x}$):** $85.91$
* **Standard Deviation ($\sigma$):** $5.58$

---

## 3. Step-by-Step Solution: Trimmed Dataset ($N = 9$)

### Step 1: Identify and Remove the Extreme Outliers
* **Lowest Score:** $77$
* **Highest Score:** $95$

Removing these two values leaves us with a new sample size of $N = 9$.
$$\text{New Dataset: } \{88, 92, 79, 85, 81, 86, 90, 83, 89\}$$

### Step 2: Calculate the New Sum and New Mean ($\bar{x}_{\text{new}}$)
$$\sum x_{\text{new}} = 945 - (77 + 95) = 773$$
$$\bar{x}_{\text{new}} = \frac{773}{9} \approx 85.8889$$

### Step 3: Compute the New Squared Deviations from the New Mean
Subtract the new mean ($85.8889$) from each remaining score and square the result:

| $x_i$ | Deviation $(x_i - 85.8889)$ | Squared Deviation $(x_i - \bar{x}_{\text{new}})^2$ |
| :---: | :-------------------------: | :-----------------------------------------------: |
| 88    | $+2.1111$                   | $4.4567$                                          |
| 92    | $+6.1111$                   | $37.3455$                                         |
| 79    | $-6.8889$                   | $47.4570$                                         |
| 85    | $-0.8889$                   | $0.7901$                                          |
| 81    | $-4.8889$                   | $23.9013$                                         |
| 86    | $+0.1111$                   | $0.0123$                                          |
| 90    | $+4.1111$                   | $16.9011$                                         |
| 83    | $-2.8889$                   | $8.3458$                                          |
| 89    | $+3.1111$                   | $9.6790$                                          |
| **Sum**|                            | **$\sum (x_i - \bar{x}_{\text{new}})^2 = 148.8888$**|

### Step 4: Calculate the New Variance and Standard Deviation ($\sigma_{\text{new}}$)
Divide the sum of squared deviations by $N - 1$ ($9 - 1 = 8$):
$$\text{Variance}_{\text{new}} = \frac{148.8888}{8} = 18.6111$$

Take the square root of the new variance:
$$\sigma_{\text{new}} = \sqrt{18.6111} \approx 4.3141$$

Rounding to two decimal places:
* **New Mean ($\bar{x}_{\text{new}}$):** $85.89$
* **New Standard Deviation ($\sigma_{\text{new}}$):** $4.31$

---

## 4. Summary of Results Matrix

| Statistical Metric | Original Dataset ($N=11$) | Trimmed Dataset ($N=9$) |
| :--- | :---: | :---: |
| **Mean ($\bar{x}$)** | **$85.91$** | **$85.89$** |
| **Standard Deviation ($\sigma$)** | **$5.58$** | **$4.31$** |

### Insight:
While the average score remained almost identical (dropping by just $0.02$), the standard deviation decreased noticeably from $5.58$ to $4.31$. This demonstrates that removing extreme outliers reduces variability, indicating that the remaining scores are more tightly clustered around the mean.
