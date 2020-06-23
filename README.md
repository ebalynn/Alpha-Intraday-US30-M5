# ScalpingIntradayUS30M5
Intraday scalping strategy written for US30 CFD. The approach will be to use SPX500 as a proxy to validate sudden moves and use ML.NET to contribute to decision making. It is based on 5M intervals for candlestick pattern recognition, however the data is received every tick. It is expected that the positions will be closed outside of trading hours, however this option is configurable.