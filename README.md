# Assignment_3_Predictive_analysis
Advance Mathematics by Dr. Suresh
(Probability Density Function Learning using Non-Linear Transformation)

## Objective

The objective of this assignment is to learn parameters of a probability density function after applying a roll-number-dependent non-linear transformation on air quality data.

---

## Dataset

India Air Quality Dataset (Kaggle)

Feature used: **NO₂ concentration**

---

## Methodology

### Step 1 — Transformation

Each value of NO₂ (x) is transformed into z using:

[
z = x + a_r \sin(b_r x)
]

For roll number **102303225**:

[
a_r = 0.15
]
[
b_r = 0.3
]

---

### Step 2 — Probability Density Function

The following function was learned:

[
\hat{p}(z)=c e^{-\lambda(z-\mu)^2}
]

This represents a Gaussian-type distribution.

---

### Step 3 — Parameter Estimation

Parameters were estimated using statistical estimation:

[
\mu = mean(z)
]
[
\lambda = \frac{1}{2\sigma^2}
]
[
c = \frac{1}{\sqrt{2\pi\sigma^2}}
]

---

## Results

| Parameter | Value         |
| --------- | ------------- |
| μ         | 25.804484510102007 |
| λ         | 0.0014602636800887954 |
| c         | 0.02155960031650373 |

---

## Graph

The histogram of transformed data closely matches the estimated probability density function curve.

---

## Conclusion

The non-linear transformation modifies the distribution of NO₂ values.
The estimated Gaussian-type probability density function successfully models the transformed variable.

---
