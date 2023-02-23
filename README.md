# Kickstarting with Excel

## Overview of Project

### Purpose
The purpose for the analysis was to help Louise compare how different crowd funding campaigns fared in relation to their launch dates and fundraising goals to her own campaign for her play "Fever" which came close to its fundraising goal of $10,000 in a short amount of time. Louise initially asked us to help her with analyzing crowdfunding data to determine whether there are specific factors that make a project's campaign successful. 

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
In performing our analysis of the "Kickstarter" data, we first added a column, column U, titled "Years" which extracted just the year from column S, "Date Created Conversion". This was added to assist in evaluating if the year affected the outcomes. We then created a pivot table in the tab "Theater Outcomes by Launch Date" to enable us to examine the different trends in the data. We adjusted the pivot table fields to visualize the campaign outcomes "successful", "failed", and "canceled" based on the launch date of the campaign. We filtered the resulting pivot table to only include campaigns with the parent category "theater" so we can better compare the "Fever" campaign to the relevant campaigns. To help us visualize the trends, we added a dynamic line chart based on the pivot table below.

![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/114427019/198102354-e847a8e4-8caa-4451-b8b3-36ec42915a30.png)

### Analysis of Outcomes Based on Goals

For our analysis in comparing the outcomes "successful", "failed", and "canceled" based on a campaign's goal, we created a new sheet called "Outcomes Based on Goals" to hold our data. We then created a table with the following columns: Goal, Number Successful, Number Failed, Number Canceled, Total Projects, Percentage Successful, Percentage Failed, and Percentage Canceled. We then created groups of dollar-amount ranges for campaigns based on their goal amount. The goals started with campaigns that were less than $1,000 and then went up in increments of $5,000. The highest group was for projects with goals $50,0000 or more. We then populated the "Number" columns of the table using `COUNTIFS()` functions to count the results that fell into each range and outcome. We also included in the `COUNTIFS()` a count for the "Subcategory" column, column R, to only count campaigns categorized as "plays". After that, we summed the count of the projects per goal range in the "Total Projects" column using the `SUM()` function. The "Total Projects" column was subsequently used to help populate the remaining "Percentages" columns. finally, we created the line chart below to visualize the relationship between the goal-amount ranges and the percentage of successful, failed, and canceled campaigns.

![Outcomes_vs _Goals](https://user-images.githubusercontent.com/114427019/198126645-1664fca0-87b1-43b8-b22d-be919f4e53d8.png)

### Challenges and Difficulties Encountered
A challenge in this analysis was making sure that the correct columns and values for each range were in the right order for the analysis of "Outcomes Based on Goals". This was difficult because each cell required a different monetary range as well as a different outcome assigned to each. It was also difficult because depending on how the `COUNTIFS()` arguments were structured, the formula may not return the correct value. Thus, getting the parameters in the correct order was also tricky.

## Results

### Conclusions About the Outcomes Based on Launch Date

Based on our analysis, campaigns created in May were more successful than any other month in the year while the worst month to start a campaign was in December. Overall, the theater crowdfunding campaigns were generally successful more often than not.

### Conclusion About the Outcomes Based on Goals

Generally, the higher the goal, the more likely the campaign was likely to fail. In comparison with Louise's campaign, it is somewhat surprising that her campaign came close to its goal but ultimately didn't reach it. Based on the trends depicted in the graph, her campaign had a slightly higher chance of succeeding rather than failing.

### Limitations of this Dataset
The data set is quite outdated. The most recent date in column T, "Date Ended Conversion", is May 3, 2017. As of this year, 2022, the data set is about five years old. This means the trends shown could be inaccurate which would lead to incorrect assumptions and faulty recommendations.

### Other Possible Tables and/or Graphs
An overall outcome analysis based on the Parent Category "Theater" based on the goals for the campaigns rather than just the Subcategory "play". This would help us better compare the "Theater Outcomes Based on Launch Date" analysis to the "Outcomes Based on Goals" analysis because we would be comparing the same data to the same data rather than just a subset of data.
