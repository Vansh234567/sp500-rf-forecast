# ML-Based Trading Strategy Comparison

## Problem Statement
This project evaluates whether machine learning models can generate profitable trading strategies on financial time series data, beyond simple buy-and-hold benchmarks.

## Data
- Asset: S&P 500 Index
- Frequency: Daily
- Period: 2015–2024
- Features: Technical indicators and lagged returns

## Models Evaluated
- Ridge Regression (baseline linear model)
- Random Forest (tree-based non-linear model)
- LSTM (sequence-based deep learning model)

## Key Results
| Model | Target | Buy & Hold % | Strategy % |
|------|-------|--------------|------------|
| Ridge | Returns | 38.4 | 0.44 |
| Random Forest | Returns | 38.4 | 196.2 |
| LSTM | Price | 33.5 | 34.0 |

*Note: Buy-and-hold returns differ slightly due to model-specific test windows.*

## Key Insights
- Lower prediction error does not guarantee profitable trading.
- Tree-based models produced the most tradable signals.
- Deep learning models require careful signal calibration.

## Disclaimer
This project uses idealized backtesting assumptions and does not account for transaction costs or slippage.
