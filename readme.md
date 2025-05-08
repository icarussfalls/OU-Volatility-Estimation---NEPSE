# Modelling Stock Volatility with Ornstein-Uhlenbeck Process

This project demonstrates how to model stock volatility using the Ornstein-Uhlenbeck (OU) process, a stochastic process widely used in financial mathematics. The notebook explores concepts such as volatility clustering, maximum likelihood estimation (MLE), and simulation of the OU process.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Requirements](#requirements)
- [Usage](#usage)
- [Key Concepts](#key-concepts)
- [References](#references)

## Overview
The project analyzes stock price data to study volatility clustering and models the volatility using the Ornstein-Uhlenbeck process. It includes:
- Exploratory data analysis of stock prices.
- Calculation of log returns and their autocorrelation.
- Maximum likelihood estimation for normal and OU processes.
- Simulation of the OU process using both continuous and discretized approaches.

## Features
- **Volatility Clustering Analysis**: Visualize and analyze daily log returns and their squared values.
- **Maximum Likelihood Estimation (MLE)**: Estimate parameters for normal and OU processes.
- **Simulation**: Simulate the OU process using both continuous and Euler-Maruyama discretization methods.
- **Visualization**: Generate plots for log returns, volatility, and simulated paths.

## Requirements
The project requires the following Python libraries:
- `numpy`
- `pandas`
- `matplotlib`
- `scipy`
- `statsmodels`
- `pandas_datareader`
- `IPython`

To install the required libraries, run:
```bash
pip install numpy pandas matplotlib scipy statsmodels pandas_datareader
