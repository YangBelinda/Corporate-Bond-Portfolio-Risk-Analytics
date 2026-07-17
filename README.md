# Corporate Bond Portfolio Risk Analytics

A Python-based fixed income risk analytics project that evaluates the market risk of an investment-grade corporate bond portfolio using historical market data. The project applies Value at Risk (VaR), Expected Shortfall (ES), interest rate sensitivity analysis, and historical stress scenario analysis to assess portfolio risk under both normal and stressed market conditions.

## Project Overview

This project analyzes the market risk of an investment-grade corporate bond portfolio using publicly available market data from the iShares iBoxx $ Investment Grade Corporate Bond ETF (LQD) and the U.S. 10-Year Treasury yield.

The analysis follows a practical risk management workflow, including data preparation, exploratory data analysis, historical risk measurement, interest rate sensitivity analysis, and historical stress scenario analysis. Together, these techniques provide a comprehensive assessment of portfolio risk and demonstrate how multiple complementary risk measurement techniques can be combined to support fixed-income portfolio risk management.

## Dataset

The analysis is based on publicly available market data:

| Dataset | Description | Source |
|---------|-------------|--------|
| LQD ETF | Daily Net Asset Value (NAV) of the iShares iBoxx $ Investment Grade Corporate Bond ETF | iShares by BlackRock |
| U.S. 10-Year Treasury Yield | Daily Treasury yield used for interest rate analysis | FRED (Federal Reserve Economic Data) |

The dataset consists of daily market observations and serves as the basis for return calculation, risk measurement, interest rate sensitivity analysis, and historical stress scenario analysis.

## Methodology

The project follows the workflow below:

```text
Data Collection
        │
        ▼
Data Cleaning
        │
        ▼
Exploratory Data Analysis
        │
        ▼
Historical Risk Measurement
        │
        ▼
Interest Rate Sensitivity Analysis
        │
        ▼
Historical Stress Scenario Analysis
```

Each stage is designed to evaluate portfolio risk from a different perspective, providing a comprehensive assessment of market risk for an investment-grade corporate bond portfolio.

| Step | Description |
|------|-------------|
| Data Collection | Collect daily LQD ETF NAV data and U.S. Treasury yield data from publicly available sources. |
| Data Cleaning | Clean, align, and merge datasets for analysis. |
| Exploratory Data Analysis | Analyze return distribution and summarize key portfolio characteristics. |
| Historical Risk Measurement | Calculate annualized volatility, Value at Risk (VaR), and Expected Shortfall (ES). |
| Interest Rate Sensitivity Analysis | Estimate portfolio sensitivity using modified duration and interest rate shock scenarios. |
| Historical Stress Scenario Analysis | Evaluate portfolio performance during the 2022 Federal Reserve tightening cycle and compare it with the full sample period. |

## Key Results

The project produced the following key outcomes:

- Quantified portfolio market risk using annualized volatility, Value at Risk (VaR), and Expected Shortfall (ES).
- Estimated the portfolio's price sensitivity under +50 bp, +100 bp, and +200 bp interest rate shock scenarios using modified duration.
- Compared portfolio risk during the 2022 Federal Reserve tightening cycle with the full sample period, showing higher downside risk under stressed market conditions.
- Demonstrated an end-to-end Python workflow for fixed-income portfolio risk analysis using publicly available market data.

## Skills Demonstrated

### Programming & Data Analytics
- Python
- Pandas
- NumPy
- Matplotlib
- Jupyter Notebook
- Data Cleaning and Integration
- Exploratory Data Analysis (EDA)

### Financial Risk Analytics
- Fixed Income Portfolio Analysis
- Value at Risk (VaR)
- Expected Shortfall (ES)
- Modified Duration
- Interest Rate Sensitivity Analysis
- Historical Stress Scenario Analysis

## Future Improvements

Potential enhancements to this project include:

- Incorporate credit spread risk to better capture changes in corporate bond valuations.
- Include convexity analysis to improve price sensitivity estimation under larger interest rate shocks.
- Apply Monte Carlo simulation to estimate portfolio risk under a wider range of market scenarios.
- Develop multi-factor stress testing by jointly considering interest rate, credit spread, and liquidity shocks.
- Extend the analysis to bond-level holdings for more detailed portfolio risk attribution.