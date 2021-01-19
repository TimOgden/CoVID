# CoVID
Data analysis on covid-19

Currently, just one analysis. I used county-level data from the 2020 presidential election, covid cases and deaths from the CDC, and populations from the 2010 Census to conduct a study of how correlated the partisanship of a county and its susceptibility to CoVID-19 is.

In this notebook, I compare and chart the number of deaths and cases for every 1,000 people per district since the November election (or whatever date you choose to set) against the percentage point difference in that county. My results show a small, but definitely statistically significant correlation of r<sup>2</sup>=.08 for cases vs. partisanship and r<sup>2</sup>=.064 for deaths vs. partisanship.

![Covid cases](https://github.com/TimOgden/CoVID/blob/main/cases_since_2020Election_75days_ago.png?raw=true)

![Covid deaths](https://github.com/TimOgden/CoVID/blob/main/deaths_since_2020Election_75days_ago.png?raw=true)

While it is easy to jump to conclusions from this data, we should also consider any confounding variables, such as how a redder district typically tends to be older in average age, and age is correlated to voting Republican. Another possible factor is that, while I am scaling the data by population (so for example the thousands of deaths in LA County or New York don't drown out the many US counties that have that same number as a total population), it is likely that a person in a high-density, high-population county has much more exposure to many different people every day than someone who lives in a more rural, open area. This information would be much more difficult to normalize out of the data, but it also stands only as a counterargument to the hypothesis that redder counties have higher covid rates, so it is likely that the correlation could be even stronger assuming equal average daily exposures to strangers in all counties.
