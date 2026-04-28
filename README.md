# Monte-Carlo-Option-Pricing-model
Monte Carlo-based option pricing framework with stochastic modeling, confidence intervals, and validation against Black-Scholes
# 📊 Monte Carlo Options Pricing Engine

## 🚀 Overview

This project implements a **Monte Carlo simulation framework** for pricing financial derivatives, with validation against the analytical **Black-Scholes model**.

It demonstrates how stochastic processes can be used to estimate option prices, analyze uncertainty, and handle more complex derivatives such as **Asian options**.

---

## 🎯 Objectives

* Implement Monte Carlo simulation for **European option pricing**
* Validate results using the analytical Black-Scholes model
* Analyze **convergence behavior** of Monte Carlo estimates
* Visualize **payoff distributions** and **price paths**
* Extend the model to **path-dependent options (Asian options)**
* Quantify uncertainty using **confidence intervals**

---

## 🧠 Mathematical Background

### Geometric Brownian Motion

We assume the stock price follows:

Sₜ = S₀ · exp((r − ½σ²)t + σ√t Z)

Where:

* S₀ = Initial stock price
* r = Risk-free rate
* σ = Volatility
* Z ~ N(0,1)

---

### Option Pricing (Monte Carlo)

The option price is computed as:

Price = e^(−rT) · E[max(Sₜ − K, 0)]

Monte Carlo estimates this expectation by simulating many possible outcomes.

---

### Black-Scholes Benchmark

The analytical Black-Scholes model provides a closed-form solution for European options and is used here to **validate simulation accuracy**.

---

## ⚙️ Features

### ✅ European Option Pricing

* Monte Carlo simulation using vectorized NumPy
* Supports both **call and put options**

### ✅ Black-Scholes Validation

* Analytical pricing for comparison
* Error analysis between simulation and exact solution

### ✅ Confidence Intervals

* Quantifies uncertainty in Monte Carlo estimates
* Provides 95% confidence bounds

### ✅ Convergence Analysis

* Visualizes how estimates stabilize as simulations increase

### ✅ Payoff Distribution

* Highlights asymmetric nature of option returns

### ✅ Price Path Simulation

* Simulates multiple possible stock price trajectories

### ✅ Asian Option Pricing

* Demonstrates pricing of **path-dependent derivatives**

---

## 📈 Visualizations

The project includes:

* 📉 Monte Carlo convergence plot
* 📊 Payoff distribution histogram
* 📈 Simulated stock price paths

These visuals help illustrate:

* Convergence behavior
* Distributional characteristics
* Stochastic dynamics of asset prices

---

## 🧪 Example Output

```bash
Monte Carlo Price: 10.23
Black-Scholes Price: 10.15
Error: 0.08
95% Confidence Interval: (10.05, 10.40)
```

---

## 🛠️ Technologies Used

* Python
* NumPy
* Matplotlib
* SciPy

---


```

---

## ▶️ How to Run

1. Clone the repository:

```bash
git clone https://github.com/gbobodoelohorolamide/monte-carlo-options-pricing-model.git
cd monte-carlo-options-pricing-model
```

2. Install dependencies:

```bash
pip install numpy matplotlib scipy
```

3. Run the notebook:

```bash
jupyter notebook
```

---

## 📌 Key Insights

* Monte Carlo simulation converges to the Black-Scholes price as simulations increase
* Confidence intervals shrink with more simulations
* Option payoffs are **highly skewed**, with many zero outcomes
* Path-dependent options require **full trajectory simulation**

---

## 🔮 Future Improvements

* Variance reduction techniques (Antithetic, Control Variates)
* Barrier option pricing
* Greeks estimation (Delta, Vega)
* Performance optimization (Numba, parallelization)

---

## 💡 Author Notes

This project demonstrates core concepts in:

* Stochastic modeling
* Numerical methods
* Financial engineering
* Statistical inference

It is designed as a **portfolio-ready quant finance project**.

---

## ⭐ If you found this useful

Feel free to star ⭐ the repo or fork it!
