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

## Results

# Stocks Analysis
The stock analysis was straighforward: to compare starting and ending prices for 12 companies throughout the years of 2017 and 2018. With those prices, we would be able to see the progress for each company Steve chose to examine.

Below are the charts for 2017 and 2018 - which show the stock value for the 12 companies. As we can see 

![StocksProgress2017](stock-analysis/resources/StocksProgress2017.png)
![StocksProgress2018](/stock-analysis/resources/StocksProgress2018.png)


## Summary




## Analysis and Challenges
In the data used for our research, there were more than 4,000 records of campaigns. The target of the campaigns was diverse: from film to food, from photography to technology, from games to journalism. With such diversity, one of the challenges encountered was to make as truthful conclusions as possible, filtering data that would be most relevant.

Another challenge was to understand data - that is not always readily available. In this case, we could list two minor adjustments: dates were recorded in Unix format and had to be converted and there was just one column listing Category/Subcategory which had to be split so we could make more precise queries. 


### Analysis of Outcomes Based on Launch Date
On a first analysis, the focus was to understand how relevant Launch Date was to a successful outcome. For that, the initial mass of data was narrowed down to show only the parent category of interest (theater) and the number of outcomes were grouped according to each possible outcome (successful, failed and canceled) in a pivot table. The idea was to find if there was a pattern throughout the year - following the seasons, for instance. 

When examining the chart based on the table created, we can clearly see that May is the most promising month to launch a funding campaign like this. Not only does it have the most successful campaigns, but it is also in May that lies the biggest gap between successful and failed/canceled projects.

![Outcomes_by_Launch_Date](resources/Theater_Outcomes_vs_Launch.png)

### Analysis of Outcomes Based on Goals
The analysis based on goals, on the other hand, focused on the most successful intervals for goals. The outcomes were split in the following intervals
 * less than 1000 (<=1000)
 * greater or equal than 1000 and less than 4999 (>=1000 and <4999)
 * greater or equal than 5000 and less than 9999 (>=5000 and <9999)
 * greater or equal than 10000 and less than 14999 (>=10000 and <14999)
 * greater or equal than 15000 and less than 19999 (>=15000 and <19999)
 * greater or equal than 20000 and less than 24999 (>=20000 and <24999)
 * greater or equal than 25000 and less than 29999 (>=25000 and <29999)
 * greater or equal than 30000 and less than 34999 (>=30000 and <34999)
 * greater or equal than 35000 and less than 39999 (>=35000 and <39999)
 * greater or equal than 40000 and less than 44999 (>=40000 and <44999)
 * greater or equal than 45000 and less than 49999 (>=45000 and <49999)
 * greater or equal than 50000 (>=50000)

For this approach, we created a table by grouping (counting) the outcomes according to the goal range they first aimed. 

We tend to think that the smallest goals would be the most successful, but the data proves us wrong. Up to the 14999 window, less than 50% of the fundraisers were successful. Between 25000 and 35000, the success rate varies from 70% to 80%, which is fairly good.

![Outcomes_based_on_Goals](/resources/Outcomes_vs_Goals.png)

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
  1. The best month to start a fundraising would be clearly May. 
  2. Throughout the year, fundings for theater tend to be more successful than fail, however, in December the chances of failure and success are just the same, making December a risky choice to start a campaign.

- What can you conclude about the Outcomes based on Goals?

  As mentioned above in the analysis, the Outcome based on Goals shows that the amount being smaller does not necessarily guarantee a successful outcome given that the most successful ranges are from 25000 to 29999 and 30000 to 34999. There is one range that is 100%, but there is just one funding in that range making it not a very good example of success given we do not have a good mass of data to work with.

- What are some limitations of this dataset?

  No limitations in this dataset, however, I believe that having a larger set to analyse would give us more precise results.

- What are some other possible tables and/or graphs that we could create?

  I would try to "play" with the data in a fashion that it would list the line for each year without grouping as in the chart below. It might explain May as the apparent best launch date, but it shows clearly that the data is mainly from 2014 to 2016, the other years contributing very little. It might be interesting to understand if there is any external variable that made these three years so prosperous in terms of funding.

![Outcomes_based_on_Goals](/resources/Theater_Outcomes_vs_Launch_by_Year.png)


