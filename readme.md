# Modelling Stock Volatility with Ornstein-Uhlenbeck Process

This repository contains a Jupyter Notebook that demonstrates how to model stock volatility using the Ornstein-Uhlenbeck (OU) process. The project explores volatility clustering, maximum likelihood estimation (MLE), and simulation of the OU process using both continuous and discretized methods.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Requirements](#requirements)
- [Usage](#usage)
- [Key Concepts](#key-concepts)
- [References](#references)
- [License](#license)

## Overview
The project analyzes stock price data to study volatility clustering and models the volatility using the Ornstein-Uhlenbeck process. It includes:
- Exploratory data analysis of stock prices.
- Calculation of log returns and their autocorrelation.
- Maximum likelihood estimation for normal and OU processes.
- Simulation of the OU process using both continuous and Euler-Maruyama discretization methods.

## Features
- **Volatility Clustering Analysis**: Visualize and analyze daily log returns and their squared values.
- **Maximum Likelihood Estimation (MLE)**: Estimate parameters for normal and OU processes.
- **Simulation**: Simulate the OU process using both continuous and Euler-Maruyama discretization methods.
- **Visualization**: Generate plots for log returns, volatility, and simulated paths.

## Requirements
The following Python libraries are required:
- `numpy`
- `pandas`
- `matplotlib`
- `scipy`
- `statsmodels`
- `pandas_datareader`
- `IPython`

Install the dependencies using:
```bash
pip install numpy pandas matplotlib scipy statsmodels pandas_datareader
```

## Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/icarussfalls/OU-Volatility-Estimation---NEPSE.git
   cd OU-Volatility-Estimation---NEPSE
   ```

2. Open the Jupyter Notebook:
   ```bash
   jupyter notebook stock-volatility-with-ou-process.ipynb
   ```

3. Run the cells in the notebook to:
   - Import stock price data.
   - Analyze volatility clustering.
   - Perform MLE for normal and OU processes.
   - Simulate the OU process.

## Key Concepts
### Volatility Clustering
- Financial time series often exhibit volatility clustering, where large changes are followed by large changes and small changes by small changes.

### Ornstein-Uhlenbeck Process
- A mean-reverting stochastic process described by:
  
  \[
  dX_t = \kappa (\theta - X_t) dt + \sigma dW_t
  \]
  
  where:
  - \( \kappa \): Speed of mean reversion.
  - \( \theta \): Long-term mean.
  - \( \sigma \): Volatility.
  - \( W_t \): Wiener process.

### Maximum Likelihood Estimation (MLE)
- Estimates the parameters by maximizing the likelihood function:
  
  \[
  L(\theta | x) = \prod_{i=1}^{n} f(x_i | \theta)
  \]
  
  or by maximizing the log-likelihood.

### Simulation
- The notebook simulates the OU process using:
  - **Continuous Formulation**: Based on the integral representation.
  - **Euler-Maruyama Discretization**: An approximate method for simulating SDEs.

## References
- Rama Cont (2005). *Volatility Clustering in Financial Markets: Empirical Facts and Agent-Based Models*.
- B. B. Mandelbrot (1963). *The Variation of Certain Speculative Prices*, Journal of Business.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

Feel free to contribute by opening issues or submitting pull requests!
