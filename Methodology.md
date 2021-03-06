1. The website through which we are obtaining our Police Violence data is ‘Fatal Encounters’, and so the first step was downloading the data. 
2. The dataset is divided into 26 columns with each case of police brutality given an unique ID number. We removed the unique ID number as this correlated to cases when all 52 states were included
3. To clean the data, we first duplicated the page and organised the sheet by state so that we could remove the cases not in our jurisdiction 
4. Given our focus is on police brutality regarding race, we then organised by race so we could isolate the cases that were against african american/black people 
    1. Some of the victim’s races were unknown and had been clarified with imputations - we kept those who were categorised as African American/black through imputations and removed the rest of the figures. This can cause further limitations to our data and were often cases that were 
5. We deleted the more specific aspects of location but kept the state and county to see if there were any specifc locations within and between states that evidenced more cases
    1. We followed a similar logic with the agency involved 
6. We also deleted columns relating to the nature of the incident, related media coverage, and the disposition of the officers involved 
7. Age and Gender were then removed 
8. Any cases outside of our time period were also removed
9. We also removed the relationship of cases with mental health 

1. To create the sheet to analyse and compare our data sets, we then made a summary of the number of cases per state in the time period (overall and per year) 
2. Next to each column, we then took the population of each state per year to ensure that we were making relative comparisons - these were taken from the US census 
    1. We compared with total population and African American/black demographics  
    2. Using the census’ CPS tool (https://www.census.gov/cps/data/cpstablecreator.html), we refined the US population by state and demographic for each year and transferred this over to our sheet 
3. We had split the responsibility of each data set between people, so after making an additional category by each year for hate crime statistics, the two people working on cleaning the data sets came together and combined their findings 


<h3>Limitations: </h3>
- public reports of cases of police brutality against civilians are notoriously under reported, especially with relation to race related incidents, therefore, most cases have been recorded from news articles 

After encountering a range of issues with our hate crime data, we, unfortunately, had to change the direction of our project. As previously explained, we made a summary of all the cases of police brutality against specifically African American/Black people in our chosen states in each year. With the hate crime data, it was impossible to reliably combine the data sets they had together to find the number of cases against African American/black people in each state each year. Instead, we were only able to obtain data that showed hate crimes towards back/african American people on a national level (all states) or the total race related crimes for each state. Inconsistencies in reporting and agencies involvement each year also caused further limitations with this. 

Given our hate crime data set was unusable, we decided instead to focus on whether there were any trends between levels of police funding per capita in each state and the levels of police brutality as we were able to find a useful data set from the Tax Policy Center. The tax policy centre is run by the Urban Institute & Brookings Institutions and they had completed data collection in 2020 for ‘state and local general expenditures 2014-2017’. Due to the new direction and data sets, we have changed our investigation to looking into all 52 states to try and account for some more of the variables involved in our areas like crime rates, population density, political ideologies etc. In addition, we needed to take our time range back by a year in order to have data from both sets.

To clean the data, we first downloaded the data sets and made templates for the two sheets we would be using to clean it - one for police brutality and one for state expenditure 

1. First step was downloading the data (for both data sets as we needed to re clean it)
2. To clean the data, we first duplicated the page and organised the sheet by data so that we could remove the cases not in our time period  
    1. Alaska and Hawaii were not counted in our funding data set and so we omitted these states in our police brutality data too
3. The dataset is divided into 26 columns with each case of police brutality given an unique ID number. We removed the unique ID number as this correlated to the order in which the cases were collected
4. Given our focus is on police brutality regarding race, we then organised by race so we could isolate the cases that were against african american/black people 
    1. Some of the victim’s races were unknown and had been clarified with imputations - we kept those who were categorised as African American/black through imputations and removed the rest of the figures. This can cause further limitations to our data and were often cases that were 
5. We deleted the more specific aspects of location but kept the state and county to see if there were any specifc locations within and between states that evidenced more cases
    1. We followed a similar logic with the agency involved 
6. We also deleted columns relating to the nature of the incident, related media coverage, and the disposition of the officers involved 
7. Age and Gender were then removed 
8. Any cases outside of our time period were also removed
9. We also removed the relationship of cases with mental health 
10. We then counted each state and the number of cases in each year of our period to put on a separate sheet ready for analysis
    1. We also totalled the cases in the US each year

For state funding, the data was in sheets based on each year from 2017 to 2000. On each sheet, figures were categorised by direct and interstate funding. We used the direct figures and took the total funding as well as the funding to the police for each state in each year. Figures were per capita.


<h3>Our Methods - REVIEWED</h3>

Our methodology is divided into three main parts which guide you through the process we followed for our project:

To answer our research question we aimed to: 
to study the evolution of police brutality against African American/Black people 
to study the evolution of funding allocation 
to compare and analyze the results

Phase 1: Descriptive statistics 

The first phase of our project was to use descriptive data to inform the trajectory of our project and how we would approach our aims to discuss the correlation between the allocation of funding and police brutality in each state of the US. We exclude Hawaii and Alaska because there was not sufficient data for the levels of funding.

Visualisation n*1 illustrates the density of the Black/African American population by state
Visualisation n*2 illustrates the number of fatal encounters per 10,000 African American/Black people
Visualisation n*3 shows police funding relative to social funding (welfare and education spending) per capita

Visualisation n*1 -  density of Black population by states 

WHY?
This map enables an overall understanding of the spread of African American/black population in the US. This visualization provides an opportunity to compare with the two other maps, to observe whether they are similar or opposed patterns.  

HOW?
We used the demographic dataset provided by the U.S Census Bureau.
We used the ‘using the census’ CPS tool to refine the US population by state and demographic, we refined the US population by state and demographic for each year and transferred this over to our sheet. 
-> Ikaay’s part about the code and how he created the map based on the data collected.

Visualisation n*2 - number of fatal encounters per 10,000 African American/black people

WHY?
This map focuses on police brutality. It provides an overall understanding of the situation of police brutality against the African American community in the US. We believe it is an interesting introduction to grasp the breadth of the issue in the US, and to identify how states are more or less targeted. 
HOW?
We used the dataset provided by the website Fatal Encounters and the U.S Census Bureau
We cleaned the dataset to isolate the cases that were against African American/black people by state in 2017
The data was originally categorised using 26 different columns and each case of police brutality was given a unique ID number. We removed this and other similar categorising information like specific aspects of location (county, zip code, geographical coordinates), the nature of the incident, related media coverage, disposition of the officers involved, age, gender, mental health. 
We kept the column about the victim’s race (and those categorised using ‘race with imputations’), but removed those that concerned cases that didn’t affect african american/black people. 
Similarly, we kept the column about the data of injury but only kept the cases that occured in 2017.
We reorganised the cleaned data in google sheet, and created a column that indicated the number of police brutality cases in 2017 by states. 
We added another column to the google sheet in which we transferred census data previously collected for the first visualisation. This normalizes the data and ensures that we are making relative comparisons.
We created the column “2017 - Cases per 10000 african american/black” where we calculated the ratio of police brutality cases per 10000 African American/Black by states in 2017. 
Visualisation n*3 - police funding relative to social funding 

WHY? 
	This map focuses on the relation of police funding and social funding, which gives us a geographical understanding of funding allocation across the states. We would be able to target the states that prioritize more or less police funding compare to social ones 
This visualization shows the different proportion of police funding compared to social ones. How does it inform our project ?  
(--> Are there big differences across the states? Are there geographic patterns that reappear and correlate to other factors/maps we look at?)

HOW? 
We used the dataset provided by the website US Tax Policy Center:
We download the dataset, that provides information about funding repartition by state and by county and by type of expenditure per capita 
We cleaned the data to isolate police funding and social funding by states in 2017. We kept the columns that provided funding allocation in (1) Public welfare (2) Elementary and Secondary Education and (3) Police 
We removed the data concerning the county.
We reorganized the data collected in a google sheet, with each column corresponding to a type of expenditure. 
We created the column “2017 - ratio police funding” where we calculated the ratio of Total Police Funding Relative Education and Welfare
Phase 2: Statistical overview 
The second phase of our project was to further inform our descriptive analysis by adding a statistical basis. While looking at patterns across the different maps, a linear regression will either confirm first previews or challenge it and may even reveal trends that we didn’t notice. Again we excluded Hawaii and Alaska because there was not sufficient data for the levels of funding.

Visualisation 4: Linear regression of the funding ratio regarding Fatal Encounters
WHY? 
	This graph will allow us to have a statistical overview of the relationship between the ratio of police funding and of fatal encounters against African American/Black people in 2017. While our project benefits from the illustrative aspects of maps, this visualization will bring a more statistical aspect to our analysis, and show if there is a global relationship at the United States scale

HOW?
We used the data from the previous sheet created for the visualisation 1 and 2
In the data sheet created for the visualization n*2 we selected the column “2017 - Cases per 10000 african american/black” 
In the data sheet created for the visualization n*3 we selected the column  “2017 - ratio police funding”
We added both column on a seperate sheet that constitute the dataset for this visualisation
Based on our descriptive statistics and the mapping we had done, we realised that studying the evolution of funding allocation in each state from 2012 to 2017 resulted in a very complex visualization, impacting the quality of our analysis. Consequently, we came to the decision that we would narrow our scope of investigation and focus on several states of the US. To choose our states, we determined a criteria of selection: funding. We decided to pick 6 states, three with the highest ratio of police funding relative to social funding, and 3 with the lowest ratio. Leaving us with Florida, Nevada and Arizona (highest ratio), and Arkansas, Kentucky and West Virginia (lowest ratio). 
Visualization n*5: Bar chart
WHY? 

The bar chart is the first descriptive visualization of our case study. It gives a first overview of the 6 states funding and fatal encounters in 2017. On one side there are the rate of police, welfare and education funding and on the other side the number of fatal encounters. This visualization is a way to notice trends that we would further study when looking at the evolution of such rates. 


HOW?
We used the data from the previous sheet created for the visualisation 1 and 2
We copied the dataset of visualization 2 to collect the data for fatal encounters 
We cleaned the states that don’t fit in the case study, keeping Florida, Nevada, Arkansas, Kentucky, West Virginia 
We copied the dataset of visualization 3 to collect the dataset for police funding
We cleaned the states that don’t fit in the case study, keeping Florida, Nevada, Arkansas, Kentucky, West Virginia 

Visualization 6: Evolution from 2012 to 2017 of Police Funding as a Percentage of Welfare and Education funding and fatals encounters against African American/Black for 6 States

WHY?
This visualization showcases the evolution of fatal encounters and allocation funding between police and the sum of welfare and education. Comparing the evolution in time of both features will allow us to notice any trends and correlation. Our aim with this graph is to see if when police funding rise or decrease, police brutality shift in a way or another 

HOW? 
We used the data provided by the websites US Tax Policy Center and Fatal encounters.
We duplicated the sheet created for both map visualizations (one about funding and the other one about fatal encounters)
For the dataset on fatal encounters 
We cleaned all the states that don’t belong to the case study and we deleted the column about demographics and ratio. 
We added a column for each year from 2012 to 2017 and found the value in the same way as we did for the first map about fatal encounter
For the dataset on funding allocation
We cleaned all the states that don’t belong to the case study.
We added a column for each year from 2012 to 2017 and added the data in the same way as we did for the second map about funding 
