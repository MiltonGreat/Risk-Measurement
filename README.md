# Exchange Rate Risk Analysis: VaR & Expected Shortfall

![screenshot-localhost_8888-2025 04 05-17_27_08](https://github.com/user-attachments/assets/5e76b9ac-8d74-4cec-bc36-cdc2a3eb506b)

### Project Overview

This project quantifies exchange rate risk using Value-at-Risk (VaR) and Expected Shortfall (ES) to measure potential losses in a portfolio exposed to currency fluctuations.

### Data Source

The analysis uses the "global_crisis_data" dataset, which contains historical information on various types of financial crises, sovereign defaults, inflation rates, exchange rates, and other economic indicators across multiple countries and time periods.

### Key Features

- Parametric & Historical VaR – Estimates worst-case losses at 95% confidence.
- Expected Shortfall (ES) – Measures average loss beyond VaR.
- Exchange Rate Simulation – Models portfolio returns under FX risk.
- Visualization – Plots return distribution with VaR/ES thresholds.

### Methodology

1. Simulated Data
- Generated synthetic exchange rates (exchange_rates) and portfolio returns (portfolio_returns).

2. Risk Metrics
- VaR: Calculated via:
- Parametric method (normal distribution).
- Historical quantile (non-parametric).
- ES: Average loss when VaR is breached.

3. Visualization
- Histogram of returns with VaR/ES marked.

### Results

- Parametric VaR (1.81%)	Max loss under normality assumption.
- Historical VaR (1.83%)	Empirical 5% worst-case loss.
- Expected Shortfall (0.0%) (adjusted: 2.5%)

### Future Enhancements

- Real Data Integration: Use historical FX rates (e.g., EUR/USD).
- Advanced Models: GARCH for volatility clustering, Monte Carlo simulation.
- Machine Learning: LSTM for predicting tail risks.

### Source

[Global Crisis Dataset from Kaggle](https://www.kaggle.com/datasets/ayush12nagar/global-crisis)
