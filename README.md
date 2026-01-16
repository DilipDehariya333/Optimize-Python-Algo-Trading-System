# Optimize-Python-Algo-Trading-System
Optimize Python Algo Trading System
I have an existing algo that routes orders to Angel One through their Smart API, I trade intraday only in Nifty options by my predefined strategy, I run a Python algo trading system that streams real time quotes directly from my broker's API connected with AWS.

My strategy is based on the closing rate of 2 minutes timeframe's candle and the closing value of Vwap indicator, but I am facing a problem, my algo not reading and picking candle's closing rate and indicator's closing value correctly, that's why algo not placing correct execution rate and not placing correct Stop Loss orders. For example – I need to place Stop Loss order of some closed candle’s high rate, if candle’s high is 88.80, so algo must place an order of exact 88.80, currently my algo is placing inaccurate rate like 88.05, 88.20, 88.50

Your task is to inspect the existing Python code that listens to the API stream, then correct whatever is causing, the core logic will stay untouched.

And I need one correction in my algo, At 15:14:59 time, the square - off (Exit) order will be placed for all existing open positions at the market rate in an instant micro second and all pending Stop Loss orders will be cancelled automatically.
