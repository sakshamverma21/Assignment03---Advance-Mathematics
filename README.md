# Learning Probability Density Function using Non-Linear Transformation

## 1. Methodology
- NO₂ concentration values are extracted from the air quality dataset and missing entries are removed.
- Each value is transformed using a roll-number-based non-linear function:
  z = x + a_r sin(b_r x)
- The transformed data is modeled using the probability density function:
  p̂(z) = c · e^(−λ(z − μ)²)
- The parameters are estimated using direct statistical computation without optimization.

## 2. Description
This assignment focuses on estimating the parameters of a probability density function after applying a non-linear transformation to real-world data. Since the given probability density function corresponds to a Gaussian distribution, the mean and variance are computed directly from the transformed data, and the remaining parameters are derived analytically.

## 3. Input / Output
**Input:**  
- NO₂ concentration values  
- University roll number  

**Output:**  
- Estimated PDF parameters:
  - Mean (μ)
  - Lambda (λ)
  - Constant (c)
