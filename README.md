# An Analysis of Kickstarter Campaigns
Performing analysis on Kickstarter to uncover trends

**OVERVIEW OF PROJECT** This purpose of this project was to examine how different factors have affected the outcomes of past Kickstarter campaigns.  In particular, the effect of campaign launch time (by month) and goal amount of funding were examined.  In addition to conducting a numerical analysis in Excel, graphs were created to visualize the relationship between campaign outcome and target funding, or campaign outcome and month of campaign launch.  Although this project was completed with data from theater campaigns, the included PivotTables can be customized to show trends in campaign outcomes for many different fields (for example, tech products or films).  Understanding the trends observed in this project can help optimize future Kickstarter campaigns.

**ANALYSIS AND CHALLENGES** For deliverable #1, 1369 past theater campaigns were analyzed based on outcome and launch date.  The following PivotTable was created in order to show a complete breakdown of data:
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

While completing the challenge, certain parts of deliverable #2 were difficult for me.  When completing the COUNTSIFS() function, totaling the number of campaigns with goals <$1000 or >= $50,000 was simple enough.  However, determining the formula for the other ranges was more tricky.  Even after sorting the plays by outcome, the COUNTSIF() values were incorrect.  I tried to apply the formula in different ways for over an hour, but ultimately found that after copying the data into a new sheet I was able to obtain the correct results.  I am still not sure why this was occurring, since I used the correct formulas and the same data.  I will be sure to ask about this in the coming days.

In addition, as someone who has previously used Excel in a limited capacity, it was challenging to work with such a large dataset (4115 total campaigns).  Making copies of the data in different Excel files was useful to ensure that data remained the same through different methods of formatting and filtering.  Otherwise, I was afraid of inadvertently corrupting the data while filtering and sorting it in different ways.

**RESULTS** From the PivotTable (for Theater Outcomes by Launch Date), it appears that 839 campaigns out of 1369 (~61%) were successful in raising their goal funding.   A small percentage (3%) of theater campaigns created were ultimately canceled, and the remaining ~36% had a failed outcome.  In addition, the highest number of campaigns are historically launched in summer months (May, June, and July).

Based on the line graph, the highest proportion of successful theater campaigns occur in May.  Campaigns launched in May and June historically obtain 100% of their campaign goal, and July campaigns reach ~90% of their goal.  A steady decline in successful campaigns is seen from May until September, until a modest increase in October and another decrease until December.  A higher proportion of failed campaigns occurs in summer (May, June, July, and August) and October.  In December, there is a roughly equal proportion of successful and failed campaigns.  

When analyzing campaign outcome based on goal funding, the highest proportion of failed campaigns had goals of $45,000 - $49,999 (although only one campaign was recorded, which skews results).  Interestingly, campaigns with goals of $24,000 - $34,999 displayed more reliably high failure rates.  In contrast, the highest proprtion of successful campaigns asked for $4999 or less.  In general, campaigns with goals between $5,000 and $24,999 displayed roughly equal proportions of successful and failed campaigns. 

Potential limitations of the dataset include the lack of qualitative information about the campaign.  Campaigns with strong blurbs and experienced cast members would likely be  successful, as donors feel more confident about the result.  This may be a confounding variable.  Although we now know that the highest proprtion of successful campaigns are launched in May and have low funding goals, other factors may have influenced donors.  A well-known cast or diligently monitored campaign, for example, may be factors.

With such a large and diverse dataset, it would be interesting to understand why campaigns which asked for medium amounts of funding ($25,000 - $34,999) were the most unsuccessful.  A table of campaigns with goals between $25,000 and $34,999 could be constructed to see whether another factor (such as campaign length or country) affect this.  In addition, perhaps each play could be categorized by their blurbs (comedies, tragedies, etc.).  Since plays are so subjective, it may prove insightful to see whether different genres of plays are more successful, and even whether different genres are more successul at different times of the year (for example, comedies in summer).
