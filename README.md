# Alpha Intraday US30 M5

The intraday alpha strategy is tailored to US30 CFD. The approach will be to use SPX500 as a proxy to validate sudden moves and use ML.NET to contribute to decision making. It is based on 5M intervals for candlestick pattern recognition, however, the data is received every tick. It is expected that the positions will be closed outside of trading hours, but for those that are happy to leave red positions overnight, it's is configurable.

The main purpose of this strategy is to generate steady positive performance regardless of the directions of the market concentrating on guerilla like trading (hm, a possible name for the strategy once it's more generic) with short holding period, minimum risk and hence high Sharpe ratio. 
I believe I have a few tricks up my sleeve: 
* ML.NET - not yet sure how accurate that is going to be, but it will certainly help with candlestick pattern recognition
* Use of SPX500 to validate our trading assumptions. In a way, we are doing pairs trading but only trading US30
* Ninja Trader 8 and C#/.NET 4.8 stack is a very powerful tool, add to this Azure and we have a monster!
* I don't believe in magic, make you a billionaire next day strategies
* There are 2 more that I'm going to keep to myself for now

## Why 5M ##

As already mentioned, 5M is only going to be used to generate candlesticks. Those candlesticks contribute to the decision making process on whether to buy/sell or hold. The data itself is going to be evaluate every tick.

### Why not 1M then? ###

There is just too much noise when looking at data using this time period
