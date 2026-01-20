# btc-copytrade-backtest

This notebook implements a backtest of an algorithmic copy-trading bot 
driven by Bitcoin price action.

The strategy identifies support and resistance levels on BTC and opens 
long or short positions when BTC interacts with those levels. Instead of 
trading BTC directly, positions are executed on selected altcoins, 
assuming BTC acts as the primary market driver.

The system is designed to run multiple bot configurations in parallel, 
varying parameters such as:
- entry sensitivity around support/resistance
- correlation
- stop-loss and take-profit logic
- volume and MA parameters

Each configuration is backtested independently, allowing performance 
comparison across many bots to identify the most robust parameter 
combinations.
