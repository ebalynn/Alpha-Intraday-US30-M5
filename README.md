# Scalping Intraday US30 M5
Intraday scalping strategy written for US30 CFD. The approach will be to use SPX500 as a proxy to validate sudden moves and use ML.NET to contribute to decision making. It is based on 5M intervals for candlestick pattern recognition, however the data is received every tick. It is expected that the positions will be closed outside of trading hours, however this option is configurable.

I believe I have few tricks up my sleeve: 
* ML.NET - not yet sure how accurate that is going to be, but it will certainly help with candle stick pattern recognition
* Use of SPX500 to validate out trading assumptions. In a way we are doing pairs trading but only trading US30
* Ninja Trader 8 and C#/.NET 4.8 stack is a powerful tool, add to this Azure integration
* There are 2 more that I'm going to keep to myself for now
* I don't believe in magic, make you a billionaire next day indicators


