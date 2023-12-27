# Quant-Winter-Camp-23-Assignment-3

So for the assignment 3, you have to draft strategies using the single candlestick patterns. Try to combine as many candlestick patterns as possible and make strategies which you think would work best based on plotting the stock from the start period to the end period.

Here are the metrics which you have to calculate:

1. Returns %: If you start off with $1000, and the final value becomes $2000, the returns % would be 100 (100*(2000-1000)/1000)
2. Prepare a trade log( this should be a dataframe) containing the following columns:
    ---> Entry index of a trade
    ---> Exit index of a trade
    ---> Duration of the trade
    ---> Returns from the trade
    ---> Max drawdown for the trade ( Max drawdown is defined as the max value of the portfolio value which goes against us. Let's say you entered the trade with $1000, that means you have a portfolio value of $1000 at the start. Let's say that during the trade the minimum
   of the portfolio value attained is $800. So the Max drawdown for the trade would be (100*(1000-800)/1000) defined as (entry-min(portfolio_value))/entry.
3. When you have calculated the max drawdown for each trade calculating the maximum drawdown for the whole strategy should be simple.


   It would be better to implement stop loss. A stop loss basically fixes the maximum loss which you can bear in a trade. It's your choice if you want to implement take profit. You are free to use any other risk management measure too. Risk management measures might reduce the returns but they work well in cutting down the drawdowns. Cutting down the drawdowns in important as whenever the portfolio value decreases a trader always feels unseasiness and wants to square off the trade feeling that his portfolio value does not decrease any further.

   While creating a strategy if you are at index i, you cannot use the stock data on index (i+1) as that is not available to you. The only data available to you is till the index i.

   Use the apple stock data( ticker='AAPL') with the start date=2018-01-01 and end date=2023-01-01.

  ** Use the data from yahoo finance.

   !pip install yfinance

   import yfinance as yf

   apple=yf.download('AAPL',start date, end date)**

   AAPL is the ticker symbol for AAPL. Attaching the documentation for yfinance along with some other useful resources.

   https://pypi.org/project/yfinance/
   
   https://zerodha.com/varsity/module/technical-analysis/

   https://www.youtube.com/watch?v=K8lhUVwP60c

   https://blog.elearnmarkets.com/spinning-tops-and-doji/

   https://www.investopedia.com/terms/h/hangingman.asp
