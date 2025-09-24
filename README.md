This project estimates the fair value of Employee Stock Options (ESOs) using a Monte Carlo simulation framework and validates results with the Black–Scholes model. It demonstrates practical application of stochastic modeling, market data integration, and IFRS-aligned fair value reporting.

# Tools & Libraries

##Python: Pandas, NumPy, Matplotlib, SciPy, yFinance

##Methods: Monte Carlo Simulation, Black–Scholes Valuation, Volatility Estimation

# Process

## Data Collection:

Downloaded Nokia stock data (2018–2024) via yfinance.

Computed daily log returns and estimated annualized volatility.

## Monte Carlo Simulation:

- Simulated 1,000 price paths using Geometric Brownian Motion (GBM).

- Calculated ESO discounted payoffs over a 4-year maturity.

## Black–Scholes Benchmark:

- Implemented the closed-form formula for European call options.

- Compared results with Monte Carlo output for validation.

# Visualization & Export

## Key Results
Model	Value (per option, EUR)
Monte Carlo	1.092
Black–Scholes	1.1649

## Volatility is the main driver of ESO value.

## Monte Carlo and Black–Scholes produced consistent valuations, increasing confidence in results.

## Payoff distribution shows high probability of zero payoff but potential upside.
