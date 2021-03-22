---
layout: post
title: Investments Devlog
---

Devlog of custom investment tracking website

*March 19th, 2021*

**Devlog #1: Planning**

Overall basic plan:
1. Research web portals, APIs, and mobile apps to collect USA stock data
2. Research how to setup stock transaction accounts
3. Determine what to invest in/divide up funds.

Plan for website:
1. Tech stack: React app, NodeJS?
2. Purpose is to have quick access to check on stats of the stocks/funds I bought.
3. V1 will be pretty static, if I want to add any new funds onto dashboard will have to do manually.
4. Future plans? Add database, ability to add the stocks from user end, filter stats.

*March 20th, 2021*

**Devlog #2: Research**

Resources:
1. (https://www.nerdwallet.com/article/investing/how-to-invest-dividend-stocks)
2. (https://www.nerdwallet.com/article/investing/how-to-research-stocks)
3. (https://www.nerdwallet.com/article/investing/what-is-how-to-open-brokerage-account)
4. (https://www.youtube.com/watch?v=UE-Pys46pMk)
5. (https://www.youtube.com/watch?v=vGcOGYkttI4)

Online brokerage options:
1. Fidelity
2. TD Ameritrade
3. Charles Schwab
4. Vanguard
5. E-Trade

Mutual Funds:
1. Convenience, diversification, active management (service fees)
2. Total market fund
 
Index Funds:
1. Like mutual funds but no active management (not as much fees)
2. Automatic reinvestment
3. Expense ratios less than 0.2% 

ETFs:
1. Like index funds, but can trade anytime, whereas index is once a day

Asset Allocation:
1. Split stocks/bonds
2. Simple equation: 100 - Age = % stock allocation
3. Fancier split: 30% Domestic equity, 15% international equity, 10% emerging market equity, 15% US treasuries, 15% tips, 15% real estate

Dividend portfolio:
1. Track record
2. Look at yields - don't chase
3. Check payout ratio
4. Diversification

Investments plan?
1. Current starting funds: $6k
2. Index funds: $4k

   Plan: two index funds, [Small cap index fund](https://fundresearch.fidelity.com/mutual-funds/summary/316146182) and [Total Market index fund](https://fundresearch.fidelity.com/mutual-funds/summary/315911693), $2k each

3. Individual investments/own research/management (prob high dividend stocks): $2k

   Plan: more research into high dividend stocks, starting with the list [here](https://www.nerdwallet.com/article/investing/how-to-invest-dividend-stocks), remember to diversify

*March 21st, 2021*

**Devlog #3: Tech Research**

Finished watching basic React JS tutorials, currently looking up similar projects as reference.

API research: IEX Cloud (free), Alpha Vantage (free), Xignite, Intrinio, Polygon.io, Tradier (free)

Proof of concept: Install react app, make sure API calls work and can create the charts/tickers. Design will be afterwards.