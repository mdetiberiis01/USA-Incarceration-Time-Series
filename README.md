# USA-Incarceration-Time-Series

## Overview
With Legalization of Marijuana in some form either recreational or medical being hot topic on the 2020 election I wanted to take a closer look at the incarceration rates of people in states who have already legalized marijuana, and those who have some of the more harsh marijuana laws in the country. The states we will be taking a look at are Colorado who was the first state to legalize marijuana back in 2014, and Massachusets who legalized Marijuana in 2018, as well as Lousianna and Mississippi which have some of the countires most restictive marijuana laws, both allowing a person to arrest anyone with even small amounts in their possesion. It is speculated that in these areas poeple of color are effected disproportionatley by these laws. By looking at incarceration data from each state and forecasting incarceration rates we attempt to predict how much revenue can be saved/made from the legalization of marijuana by both additional tax revenue as well as not having to pay to house this many people in jails and prisons.

## Goals:
- To build a Time Series forecasting model to predict incarceration rates in each of these 4 states.

- By predicting the incarceration rate of people in these locations we can see if there are any trends in the two legal marijuana states and the two illegal mariajuana states pertaining to demographic.

- If we can predict the increased rate of incarceration in states without legal marijauana we can calculate how much daily cost would be for the state to house these people.

- Compare the cost of housing prisoners with the sales revenue in states that have a thriving legal marijauana market.

## The Approach
- Used the nsepy library to pull the ZEEL stock data from Jan 1, 2015 to October 22, 2020

- Engineer features to give model deeper insight

- Perform Exploratory Data Analysis on the data and create visualizations.

- Build and test ARIMA model to predict rise or fall of incarceration per state.

## Summary of Findings
- Upon looking at Colorado, a state that legalized marijauan more than 6 years ago, it was observed that the population of persons in jail was reflective of the total population broken down by demogrpahic. A similar finding is such when looking at the data from Massachusetts as well.

![](https://github.com/mdetiberiis01/Photos/blob/master/CO_jail:pop.png) ![](https://github.com/mdetiberiis01/Photos/blob/master/MA_jail:pop.png)

- Looking at Louisianna and Mississippi, we see quite the opposite. We see almost the inverse actually

![](https://github.com/mdetiberiis01/Photos/blob/master/LA_jail:pop.png) ![](https://github.com/mdetiberiis01/Photos/blob/master/MS_jail:pop.png)

- Our model performed quite well with an RMSE between 9.37 and 9.53. As you can see in the figure our predictions were quite close to the actual values. 

- In recent times, on average more days have had a higher open than close price which can be seen in the steady decline in share value since 2018.

- We predicted an opening price of $174.62 and a closing price of $181.96 for the week of 10/19/2020 and 10/23/2020, which is a good indication we should buy this week and sell before market close at weeks end.


## Business Insight
- The week of October 19, 2020 to October 23, 2020 is a good week buy shares early in the week and sell before market close on Friday.

- ZEEL has been having more days with a lower closing price than opening price since which would make us suggest looking for a new company to invest in in order to have higher returns at a faster rate. 

## Limitations and Future Work
- One main limitation would be regarding the nsepy library. The library only has a select few number of stock that allow historic data access. Because of this our model will not scale for all stocks.

- I would like to find an alternative data source so the model will be usable for more than the select few stocks.
