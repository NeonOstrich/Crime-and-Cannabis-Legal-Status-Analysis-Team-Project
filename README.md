# Project_1_Group_3: Crime & Cannabis Legality
This is a group assignment that was completed for the George Washington University Data Analytics Bootcamp, focused on analysis
and visualization in Python using Jupyter Notebook and displaying understanding of using public datasets to uncover insights.


## Organization
Within this repository you will find this "README.md" file which provides an explanation of our process and analysis. You will also find the "Project Proposal", the "cannabis_legal_status_2020" csv file, the "dirty_data" Jupyter file, and the "clean_data" csv, and our powerpoint presentation. 

In addition to these documents, we have an "Excel Files" folder which contains the original excel files which we pulled our starting data from, as well as the master excel file which all of these were put into before conversion into a csv.
There is also a folder marked "ANOVAs by Crime" which contains ANOVA analysis of the different states grouped by their cannabis legalization status. There is a "Regression Analysis" folder which contains the code and visuals of our regression analysis. And finally, there is a "Data Visualizations" folder which contains datavisualizations of each crime by state in addition to each crime by state grouped by their cannabis legalization status.

##Why Investigate?

###Multiple factors indicate that changing cannabis legal status has the potential to BOTH increase and decrease crime.

Alcohol and opioid use is thought to decrease when cannabis is available as an alternative.

There is less need for criminal cannabis organizations to use violence or carry weapons without fear of arrest.

Mass shooters have an anecdotal association with cannabis.

Major criminal organizations are thought to make the majority of their income off cannabis trafficking. Without this source they may explore more criminal alternatives.

##Investigated questions

How do crime rates differ between states?

How does cannabis legal status relate to different types of crime?

Do states with different legal statuses for cannabis have different crime rates?

How does cannabis legal status affect crime rates?

## Background

We started off our project by sourcing our 2020 crime data through the FBI, and by individually researching each state to determine its cannabis legal status in 2020 specifically. 

We determined that cannabis was illegal if there was not a medical way to access medical grade cannabis, and penalties for cannabis posession included potential prison time. We determined that cannabis was only medically legal if there was a medical way to access medical grade cannabis, but penalties for cannabis posession included potential prison time. We determined that cannabis was decriminalized if penalties for cannabis posession did NOT included potential prison time (in all of the states we looked at, decriminalized cannabis coincided with medicinal cannabis). And we determined that cannabis was recreationally available if recreational dispensaries were in operation and supplying customers. In each case, if there was a status change, the state was designated with the status that it was converting into, only if it held this status for at least 50% of the year.

The dataset that we analyzed includes 7209 datapoints which were law enforcement agencies which provided the FBI with complete data for the year 2020. It did not include Hawaii and further research revealed that almost 40% of law enforcement agencies did not submit any data in 2021, suggesting an underlying problem with the reliability of this data given how it is undermined by chronic under-reporting.

The crimes that we analyzed were Violent Crime, Rape, Robbery, Aggravated Assault, Property Crime, Burglary, Larceny-Theft, and Motor Vehicle Theft. In order to accurately compare these crimes across different states and law enforcement agencies, each value was converted to a per-capita metric.

### Research Questions

We focused on answering the following questions in order to determine the nature of the relationship (if any) between cannabis legal status and crime:

How do crime rates differ between states?

How does cannabis legal status relate to different types of crime?

Do states with different legal statuses for cannabis have different crime rates?

How does cannabis legal status affect crime rates?


### Analysis

First, we created visual representations of how often each crime occurs per capita per state. Next we created visuals of these same state comparisons, but grouped by cannabis legal status. This enabled us to see how state variability decreased within these groups, as apposed to when they were all grouped together. It also shows how some states have consistently high rates accross multiply crime types.

Next we created visuals which show how each cannabis legal status type, compares to each other type. This was in order to determine if these groups are statistically significantly different, as well as to determine what pattern that potential difference took the form of.

Finally, we created regression analyses to show the extent to which the cannabis legality distinction is causally related to crime rates across the law enforcement agencies that we analyzed.


## Insights
We can see that some states have noticibly higher crime rates in certain categories. While sometimes this is consistant across multiple crimes, it is generally crime specific or crime type specific. This suggests that some states have more problems with certain types of crimes than others, and that these crimes do not have a high degree of interrelatability.

When we group states by their cannabis legal status, we can see that the states generally have closer values to eachother. While some states rank similarly across multiple crimes, there is quite a bit of variability, suggesting that individual states are higher in certain crimes than in others, and that other states have a different distributrion of criminal activity across crimes.

We performed an ANOVA on our data in order to determine if the cannabis legal status groups were significantly different. In all of our analyses, we determined that at least one group was significantly different from at least one other, and we sometimes had as many as 5 instances of groups being significantly different. This suggests that there is a real difference between the crime rates of states with different cannabis legal statuses. 

When we graphed the means of each of these groups for each crime, a disturbing pattern emerged. This showed the trend that illegal states generally have high or medium crime rates, which decreases in the transition to medical states, decreasing further with the transition to decriminalized states, and finaly shooting up for recreational states, either to the level of illegal states, or sometimes even higher.

Finally, we performed a regression analysis by crime of cannabis legal status in relation to crime rate. This produced very low r squared values, the highest being .05. This indicates that these variables do not have a linear relationship, perhapse because they have a curved relationship.

## Possible Explanations for this pattern

Cannabis has been shown to decrease dependence on alcohol and opioids.
Decreasing penalties for possession makes it easier for medical patients, recreational users, and criminal organizations.
Recreational Marijuana sets up a competitive industry that competes DIRECTLY with the black and grey market cannabis industry.
Some of those working in the black and grey market are put out of business and need fresh streams of income, which may be more likely to be illicit.
Recreational Cannabis facilities can not use banks, setting them up to be prime targets for theft and violence.

## Directions for Future Study

Improve reporting from Law Enforcement Agencies and repeat analysis.
Repeat this analysis over multiple years and as more states adopt more lenient stances towards cannabis.
Perform a comparative analysis of law enforcement agencies in recreational states in order to discover the lowest-crime implementation strategy.
Investigate the size and practices of black and grey markets in all states.
Investigate how black and grey markets respond to changes in cannabis’s legal status.
Investigate the role of cartels, and interstate criminal networks in different states and whether this differs significantly in recreational states.


