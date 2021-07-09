# Kickstarting with Excel

## Overview of Project
We are helping Louise compare different fundraising campaigns for plays after she just tried raising money for her play called ***Fever*** 

### Purpose
For this project we are analyzing two factors and how they affected the outcomes of Kickstarter funds. On our first analysis we looked at whether the month a Kickstarter was launched affected its outcome. On the second analysis we were seeing if the amount we set our goal to discouraged or encourged people to pledge.

## Analysis and Challenges
In this analysis there were a couple of new formulas to learn along with learning to make sure the data and formulas I had were still organized
### Analysis of Outcomes Based on Launch Date
I had never done a pivot table before, so I played around with it by dragging and dropping lables until I understood the computing process.  After that I began working on the analysis without running into any issues and came out with what the deliverables asked for. **See Below** 

![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/83510059/125016678-b938c900-e03f-11eb-92fb-cf1f488914f0.png)



### Analysis of Outcomes Based on Goals
In this analysis I learned about how to use *CountIf*  function. This analysis had multiple specific parameters of both numbers and words to account for this we had to use the *CountIfs* function instead of just *CountIf*. for the analysis we needed to count successful, failed, and canceled plays in between goal amount increments of $5000 to do so the code looked like so 

***=COUNTIFS(KickStarter!$D:$D, ">=5000",KickStarter!$D:$D, "<10000",KickStarter!$F:$F, "successful",KickStarter!R:R,"plays")*** 

with small changes for specifics. After finishing all the necessary counting, I calculated the percentages to create a graph to show the successfulness of campaigns depending on goal amounts. **See Below**

![Outcomes_vs_Goals](https://user-images.githubusercontent.com/83510059/125016614-9efeeb00-e03f-11eb-92f2-8ac18714429c.png)



### Challenges and Difficulties Encountered
I noticed that a challenge someone may have with pivot tables is not knowing where to put their labels in the pivot table which would result in their data not being shown correctly or counting the wrong columns. Also an issue that I started to notice while doing the Outcomes based on Goals analysis was how time consuming it was to go through each cell and change the specicfics. However, after messing around with excel I found the find and replace command that cut my time by more than half. 
## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date? 
    - Two conclusions I can draw from the Outcomes based on Launch Date are that a person should not run a campaign during December because that had the least succes rate. the other conlusion is the a person should run their campaign in May and if not then June because those months have the highest successful counts.

- What can you conclude about the Outcomes based on Goals?
    - I can conclude from the Outcomes based Goals analysis that the goal amount does not significantly influence the outcome of a campaign.

- What are some limitations of this dataset?
    -Some limitations is that we do not account for the advertising budgets for the campaigns. Also we do not who is running the campaigns which could influence the popularity of campaign and how much traction it gets affecting the amount of backers and whether or not its successful. lastly another limitation is we do not have the genres of the plays which could also influence popularity.

- What are some other possible tables and/or graphs that we could create?
    - We could create a number of backers based of launch date line graph because that could signify when people are visiting Kickstarter. Another is seeing if having a spotlight affected success rates by creating a bar clustered bar graph showing both fails and successes.
