Title: Learning Probability Density Function using Non-Linear Transformation
1. Methodology

The NO₂ values from the given air quality dataset are first cleaned by removing missing entries. Each value is then transformed using a roll-number-dependent non-linear function:

z = x + aᵣ sin(bᵣ x)

where the constants aᵣ and bᵣ are calculated using the university roll number as specified in the assignment. After transformation, the resulting values are modeled using a probability density function of the form:

p̂(z) = c · e^(−λ(z − μ)²)

The parameters of this function are computed using direct statistical estimation.

2. Description

The objective of this assignment is to learn the parameters of a probability density function after applying a non-linear transformation to real-world data. Since the given probability density function corresponds to a Gaussian distribution, the mean and variance of the transformed data are calculated directly, and the remaining parameters are derived analytically. No optimization or machine learning techniques are used.

3. Input / Output

Input:

NO₂ concentration values from the dataset

University roll number

Output:

Estimated probability density function parameters:

Mean (μ)

Lambda (λ)

Constant (c)
