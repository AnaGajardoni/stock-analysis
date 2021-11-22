# VBA of Wall Street

## Overview of Project
Steve has just graduated with his finance degree and is helping his parents, who are passionate about green energy, to invest their money. Steve's parents decided to invest all their savings in DAQO New Energy Corp - a company that makes silicon wafers for solar panels, but Steve believes in diversification and wants to advise his parents on the best deal instead. 

### Purpose
The purpose of this project is to analyse stocks from green energy companies (including DAQO) to find out:
  - if DAQO is really the best option (or maybe even a good option)
  - learn about other green energy companies stocks as opposed to DAQO

## Technical Purpose  
On the technical side, the purpose was to refactor a macro that we had written after following the step-by-step in the online modules. According to Wiktionary, refactor in programming means "To rewrite existing source code in order to improve its readability, reusability or structure without affecting its meaning or behaviour" (https://en.wiktionary.org/wiki/refactor).
In our case, the idea was to improve our macro so as to:
- make it faster by using loops more efficiently (measured by a timer);
- make useful comments to improve readbility;
- substitute hard-coded values by variables that could be easily changed, therefore making the final code easier to mantain should a change be needed.

### Results

## Stocks Analysis
The stock analysis was straighforward: to compare starting and ending prices for 12 companies throughout the years of 2017 and 2018. With those prices, we would be able to see the progress for each company Steve chose to examine.

The summaries below show the behavior of the stocks within one year: the starting and ending price were collected for each stock and the percentage of gain was calculated. As it is clear, in 2017, only one company had a negative outcome, but, in 2018, only two had a positive one. This can mean the stocks are not doing well, but it can also mean a trend in the market. We will leave that kind of analysis to our specialist Steve!

![AllStocks2017](/resources/AllStocks2017.png)
![AllStocks2018](/resources/AllStocks2018.png)

The following charts show the exact curve within the two years we are studying. Some stocks have more ups-and-downs while others are more stable. Steve may certainly use this information as a recomendation for a more diversified portfolio. 

![StocksProgress2017](/resources/StocksProgress2017.png)
![StocksProgress2018](/resources/StocksProgress2018.png)

## Refactoring Analysis
The results for the refactoring can be easily seen the macro took to run in the two scenarios:

![AnalysisAllStocksTimer](/resources/AnalysisAllStocksTimer.png)
![AnalysisAllStocksRefactoredTimer](/resources/AnalysisAllStocksRefactoredTimer.png)



### Summary




