# An Analysis of Kickstarter Campaigns
Performing analysis on Kickstarter to uncover trends

**Overview of Project** This purpose of this project was to examine how different factors have affected the outcomes of past Kickstarter campaigns.  In particular, the effect of campaign launch time (by month) and goal amount of funding were examined.  In addition to conducting a numerical analysis in Excel, graphs were created to visualize the relationship between campaign outcome and target funding, or campaign outcome and month of campaign launch.  Although this project was completed with data from theater campaigns, the included PivotTables can be customized to show trends in campaign outcomes for many different fields (for example, tech products or films).  Understanding the trends observed in this project can help optimize future Kickstarter campaigns.

**Analysis and Challenges** For deliverable #1, 1369 past theater campaigns were analyzed based on outcome and launch date.  The following PivotTable was created in order to show a complete breakdown of data:
![image](https://user-images.githubusercontent.com/99574730/153797941-3750ae1e-9c66-410c-84e6-97ff4a7eb5fc.png)

The table was filtered by parent category (theater) and year (to separate campaigns based on month launched).  In addition, the theater campaigns were divided by outcome (successful, failed, and canceled).
A line graph was also created from the PivotTable to visually depict the trends present:

![image](https://user-images.githubusercontent.com/99574730/153798374-16a015c3-6b9f-47f2-b2d9-07426136ded4.png)

For deliverable #2, theater campaign outcomes were analyzed based on goal funding.  A table was constructed to observe the proprtion of successful, failed, and canceled campaigns depending on the target amount of funding.  Goal funding was broken into the categories within a range of $5000, with exception for goals under $1000 or over $50,000.

![image](https://user-images.githubusercontent.com/99574730/153800016-c3066ab4-6e08-4eed-81d5-9317c8d0e5e7.png)

In order to efficiently categorize such a large amount of data (1047 plays), the COUNTSIF function was used.  The data was first filtered so that only plays were displayed.  Next, the data was sorted so that failed campaigns were grouped together, as well as successful and canceled campaigns.  To calculate the number of successful plays with goals of $1000 - $4999, for example, the following formula was used:

![image](https://user-images.githubusercontent.com/99574730/153800418-6ae6566e-7eda-4be8-85b3-012c67593af2.png)

For subsequent successful plays, the same formula was applied with a different range.  For failed plays, the formula was applied to the appropriate plays from the original data.  After obtaining the number of plays in each category, proportions were calculated as a more insightful metric.

After tabulating data, a line graph was constructed to visualize the trend:

![image](https://user-images.githubusercontent.com/99574730/153799910-2a494c6e-68c1-4b7d-aa4e-89144b481417.png)

The graph was constructed by plotting the proportion of goal funding received as a function of goal funding.

**Results** From the PivotTable (for deliverable #1), it appears that 839 campaigns out of 1369 (~61%) were successful in raising their goal funding.   A small percentage (3%) of theater campaigns created were ultimately canceled, and the remaining ~36% had a failed outcome.  In addition, the highest number of campaigns are historically launched in summer months (May, June, and July).  

Based on the line graph, the highest proportion of successful theater campaigns occur in May.  Campaigns launched in May and June historically obtain 100% of their campaign goal, and July campaigns reach ~90% of their goal.  A steady decline in successful campaigns is seen from May until September, until a modest increase in October and another decrease until December.
