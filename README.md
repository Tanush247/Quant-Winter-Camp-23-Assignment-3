# Quant-Winter-Camp-23-Assignment-3 Simplified Instructions

For Assignment 3, your task is to create trading strategies using single candlestick patterns. Combine these patterns to design strategies that you believe will work well when plotting a stock from the beginning to the end of the specified period.

Here are the key things you need to do:

1. **Calculate Returns %:**
   If you start with $1000 and end up with $2000, calculate the returns percentage as \(100 \times \frac{(2000-1000)}{1000}\).

2. **Create a Trade Log (DataFrame):**
   Make a table (like a spreadsheet) with details for each trade:
    - Entry index of a trade
    - Exit index of a trade
    - Duration of the trade
    - Returns from the trade
    - Max drawdown for the trade (the biggest drop in portfolio value during the trade).

3. **Maximum Drawdown for the Whole Strategy:**
   Figure out the largest drop in value for the entire strategy based on individual trades.

It's a good idea to set up a stop loss, which is like a safety net to limit the biggest loss you're willing to take in a trade. You can choose to implement take profit or other risk management measures. While these measures might reduce profits, they help in avoiding big losses. This is important because when your portfolio value goes down, it can make you uneasy, and you might want to end the trade to prevent further losses.

Remember, when creating a strategy at a certain point, you can't use stock data from the next point. You can only use data up to that point.

Use Apple stock data with the ticker 'AAPL' and the start date as '2018-01-01' and end date as '2023-01-01.'

**Use the data from Yahoo Finance.**

```python
!pip install yfinance
import yfinance as yf

apple = yf.download('AAPL', start='2018-01-01', end='2023-01-01')
```

AAPL is just the code for Apple stock. Check out the yfinance documentation and explore additional resources to get a good grasp:

- [yfinance Documentation](https://pypi.org/project/yfinance/)
- [Technical Analysis Module - Varsity by Zerodha](https://zerodha.com/varsity/module/technical-analysis/)
- [Candlestick Patterns - elearnmarkets](https://blog.elearnmarkets.com/spinning-tops-and-doji/)
- [Hanging Man Pattern - Investopedia](https://www.investopedia.com/terms/h/hangingman.asp)

This task will help you understand technical analysis, candlestick patterns, and risk management to build effective price action trading strategies.
