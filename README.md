# An Analysis of Kickstarter Campaigns
This analysis on Kickstarter data to uncover trends was to help an playwright, Louise, to plan a crowdfunding campaign to help her fund her play, "Fever".

To start, we added two columns to hold "Percentage Funded", column O, and "Average Donation", column P, to add information to help us possibly determine, if possible, what made a successful campaign vs a failed campaign. We also added conditional formatting to column F, "outcome", to highlight successful campaigns in green, failed campaigns in red, live campaigns in blue, and canceled campaigns in yellow. We also added conditional formatting to column O, "Percentage Funded", to show the bottom number in red and the top 90% of data in blue. There were multiples of the bottom number, "0", as there were many campaigns that had goals, but nothihng was pledged during the campaign. We also cleaned the data and separted column N, "Category and Subcategory", into separate columns to aid in the filtering of the data once we drilled down to the successful and unsuccessful campaigns.

Through the analysis, we determined that May would be the best month for Louis to hold her crowdfunding campaign. Based on the followuing chart, "Outcomes Based on Launch Date", the historical data shows that successful theater crowdfunding campaigns peaked in the month of May. 

![Parent_Category_Outcomes]("C:\Users\rackl\OneDrive\Desktop\Bootcamp\Module 1 Work\Crowd Funding Analysis\Parent_Category_Outcomes.png")

In addition, it was determined that the most successful campaigns were typically smaller campaigns with a mean goal of approximately $5,000 and a median goal of $3,000. Failed crowdfunding campaigns ofthen had a significantly higher mean goal of $10,500 and a median goal of $5,000. In both the failed and successful campaigns, the data was skewed to the right.

In diving further into the data, we determeind the standard deviation and the interquartile range (IQR) of both the failed and successful campaigns. Based on this analysis, the data follows similar distributions in each subset with the mean of each distribution being around the 3rd quartile. There are also some very large values dirving the distributions. The standard deviations were all roughly twice the IQR in each distribution except in the failed Kickstarters data set.
