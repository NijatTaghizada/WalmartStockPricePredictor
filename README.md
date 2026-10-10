# Walmart Stock Price Predictor

A linear regression model that predicts Walmart's (WMT) daily closing price from its 10-day and 50-day moving averages.

- Data: `WMT.csv`, daily prices from 1972 onward
- Features: 10-day and 50-day moving averages of the close
- Split: first 77% of dates for training, last 23% for testing (not shuffled, so the model never sees the future)
- Result: RMSE of about $1.75 on the test set, roughly 4.9% of the average closing price

The notebook also plots predicted vs. actual prices.

Since moving averages are built from past prices, the model mostly follows the recent trend. It's a learning project, not something to trade with.

## Run it

```bash
pip install pandas numpy scikit-learn matplotlib
jupyter notebook main.ipynb
```
