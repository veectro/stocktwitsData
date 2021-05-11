Source : [REDDIT](https://www.reddit.com/r/algotrading/comments/n9t2w4/i_scraped_3700_stocks_from_stocktwits_every_day/)

I sorted the stocks by volume then picked the first 3700, those are the one that are scraped. There were some days (I think 4), where it crashed, so it recorded nothing that day. The first row is for the days, so you can see which days are missing. Besides that each row contains one ticker's data in the following form:

TICKER, TICKER, WASDATA, TRENDING, TRENDINGSCORE, MESSAGEVOLUME, FOLLOWERS, SENTIMENT

WASDATA is boolean that tells if if it found data for that day for that stock, if it didn't find data, then it is set to false, and the numbers after it are made up numbers

TRENDING: 0 if found it, and was true, 1 if found it and was false, 2 if it didn't find it

Currently it goes from 2021.03.27 - 2021.05.10

It always started at the same time about 20 minutes before market open, and finished before market open.

You can download it here: https://github.com/harcipulyka/stocktwitsData
