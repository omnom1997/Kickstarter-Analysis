# Kickstarting with Excel (About 1 paragraph per heading/subheading)

## Overview of Project

### Purpose
The purpose for the analysis was to help Louise compare how different crowd funding campaigns fared in relation to their launch dates and fundrasing goals to her own campaign for her play "Fever" which came close to its fundraising goal of $10,000 in a short amount of time. Louise initially asked us to help her with anyalyzing crowdfunding data to determine whether there are specific factors that make a project's campaign successful. 

## Analysis and Challenges
Explain how you performed your analysis using images and links to code, as well as any challlenges you encountered and how you overcame them. If you had no challenges, describe any possible challenges or difficulties that could be encountered

### Analysis of Outcomes Based on Launch Date (The critical evaluation which leads to the conclusion)
In performing our analysis of the "Kickstarter" data, we first added a column, column U, titled "Years" which extracted just the year from column S, "Date Created Conversion". This was added to asisst in evaluating if the year affected the outcomes. We then created a pivot table in the tab "Theater Outcomes by Launch Date" to enable us to examine the different trends in the data. We adjusted the pivot table fields to visualize the campaign outcomes "successful", "failed", and "canceled" based on the launch date of the campaign. We filtered the resulting pivot table to only include campaigns with the parent category "theater" so we can better compare the "Fever" campaign to the relevant campaigns. To help us visualize the trends, we added a dynamic line chart based on the pivot table which is included below.

![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/114427019/198102354-e847a8e4-8caa-4451-b8b3-36ec42915a30.png)

### Analysis of Outcomes Based on Goals

For our analysis in comparing the outcomes "successful", "failed", and "canceled" based on a campaign's goal, we created a new sheet called "Outcomes Based on Goals" to hold our data. We then created a table with the following columns: Goal, Number Successful, Number Failed, Number Canceled, Total Projects, Percentage Successful, Percentage Failed, and Percentage Canceled. We then created dollar-amount ranges for campaigns to be grouped based on their goal amount. The goals started with campaigns that were less then $1,000 and then went up in increments of $5,000. The highest group was for projects with goals $50,0000 or more. We then populated the "Number" colums portion of the table using `COUNTIFS()` functions to count the results that fell into each range and outcome. We also included in the `COUNTIFS()` a count for the "Subcategory" coulumn, column R, to only count campaigns that were categorized as "plays". After that, we summed the count of the projects per goal range in the "Total Projects" column using the `SUM()` function. The "Total Projects" column was subsequently used to help populate the remaining "Percentages" columns. finally, we created a line chart to visualize the relationship between the goal-amount ranges and the percentage of successful, failed, and canceled campaigns. The chart is included below.

![Outcomes_vs _Goals](https://user-images.githubusercontent.com/114427019/198126645-1664fca0-87b1-43b8-b22d-be919f4e53d8.png)

### Challenges and Difficulties Encountered
A challenge in this analysis was making sure that the correct columns and values were included in the right order for the analysis of "Outcomes Based on Goals". 

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
Campaigns created in May were more successful than any other month in the year.

The worst month to start a campaign was in December. The number of Successful campaigns and Failed campaigns were about equal.

- What can you conclude about the Outcomes based on Goals?
Generally the highetr the goal, the more likely the campaign was likely to fail.

- What are some limitations of this dataset?
The data set is quite outdated. The most recent date in column T, "Date Ended Conversion", is May 3, 2017. As of this year, 2022, the data set is about five years old. This means the trends shown could be inaccurate which would lead to incorrect assumptions and faulty recommendations.



- What are some other possible tables and/or graphs that we could create?
A overall outcome analysis based on the Parent Category "Theater" based on the goals for the campaigns
