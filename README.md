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

- Looking at Louisianna and Mississippi, we see quite the opposite. We see almost the inverse actually, where the black population has a disproportionate population inside of the states jails, compared to the much higher population of white individuals.

![](https://github.com/mdetiberiis01/Photos/blob/master/LA_jail_pop.png) ![](https://github.com/mdetiberiis01/Photos/blob/master/MS_jail:pop.png)

- It is important to remember this does not PROVE anything, but rather shows a correlation in the two instances.

- Our prediction for Colorado and Massachusetts show an swing of -44 and +78 inmates respectivley, actually predicting lower rates in many counties, while Louisianna and Mississippi both indicate much higher numbers of +1067 and +377 respectivley. 

- Massachusets forecast for example


![](https://github.com/mdetiberiis01/Photos/blob/master/MA_forecast.png) ![](https://github.com/mdetiberiis01/Photos/blob/master/MA_residuals.png)

- As an evaluation metric I used RMSE (ranging among our models from 3.8% to 13.2%)because in this type of analysis I felt it is most important to have an idea how far your prediction is away from the actual number since our prediction will be involved in future calculations.

## Business Insight
- Given the exploration of the data, the best course of action would be for more states to follow the lead of Colroado, Massachusetts, Oregon, California, and many others who have legalized marijuana.

- One of the main reason for suggesting this is becasue it can be argued that the enforcement of these policies effect communities of color at a much more higher rate, leading to more poeple being put in jail, and even if it is for just a weekend or a few days, that can turn a persons life upside down with their job and a number of other things.

- Second reason for suggesting this related to the economy, especially as we try to bounce back from this pandemic. In 2019 Colorado collected $302 Million in marijuana taxes, and Massachusetts in their first full legal year collected over $71 Million, and is expected to increase.

- Comparing this revenue to the cost that states like Louisianna and Mississippi spend on keeping people in jail, it ammounts to a huge swing. 

- According to our predictions, Louisianna and Mississippi are spending $355888.33 and $160120.80 per day to house inmates. Colorado and Massachussetts are sliughtly bigger than LA and MS, but they too could see tax reven revenue within this same window which is between $191780.82 and $827397.26 daily.

## Sourcing
- USA Incarceration Data
- https://www.vera.org/publications/price-of-prisons-2015-state-spending-trends/price-of-prisons-2015-state-spending-trends/price-of-prisons-2015-state-spending-trends-prison-spending


