Initical workflow for using screener (must be run only once - when you use the screener first time):

1. Run **get_nasdaq_stable.ipynb** and **get_nyse_stable.ipynb** scripts
   - this will create lists of "stable" traded assets on both exchanges and it will save them in respective files
2. Run **get_ohlcv.ipynb** - this will pull the history prices from the exchanges
3. Run **populate_indicators.ipynb** - this will create a folder with technical indicators
4. Now you can filter the stocks according to your logic and strategy

Typical workflow:
1. Run **update_indicators.ipynb** - this will update the indicators files up to date
2. Optional: run **update_ohlcv.ipynb** - this will update OHLCV files up to date
3. Run filter stocks logic (according to your strategy and logic)
