# Kickstarting with Excel

## Overview of Project

### Purpose

The purpose of this project was to help Louise determine whether success or failure rates of the various theater campaigns and plays are impacted by variables such as the month in which the campaigns were launched, and the dollar amounts of the goals, respectively.

Using pivot tables and -charts, we helped Louise narrow down the vizualization of her data set to only theater data and plays by filtering out other parent categories and subcategories.  We further narrowed down our analysis to filter for outcomes, months and goal amounts.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
To help vizualize the relationship between the months of the launch dates and the THEATER campaigns' rates of successes, failures and cancellations; we created a pivot chart that filtered by parent category, displayed the months on each row, and the counts of each outcome in the following columns.

The line chart linked to the filtered data shows that cancellations for theater campgains were always the smallest percentage, and successful campaigns always comprised the largest percentage for each month, regardless of the month.

The lines for successful and failed campaigns seem to follow a similar pattern from January through April.

May saw the highest count of total campaings, as well as the highest percentage of successful campaigns.

The number of both successful and failed campaigns tapers off from May through September, followed by a brief increase in October, and a continuing decline through December.

December saw the lowest total count of campaings, and was also the first month in which the percentages of successes and failures was relatively equal for the first time all year.

<img width="576" alt="Theater Outcomes Based on Launch" src="https://user-images.githubusercontent.com/106359572/174671884-12da5627-a13c-4a05-92af-42a2ff8fc513.png">

### Analysis of Outcomes Based on Goals

To help visualize the relationship between PLAY campaign outcomes and goal amounts, we grouped campaign outcomes by goal dollar amount ranges (in increments of 5,000) and then for each range, we calulated the percentages of successes, failures and cancellations by dividing their count by the total number of campaigns with goal amounts within that range.

We used the COUNTIFS function to pull the PLAY data from the kickstarter sheet and count the number of each outcome in each goal amount range.

We created a line chart to show dollar amount ranges along the x-axis and percentage of each outcome along the y-axis.  
There were no play cancellations at all, so the lines for successful and failed plays are inverseley related.

Looking only at plays that had campaign goals under $25,000, in general the lower the goal amount, the higher the chance of success.
Play campaigns with goals between $35K and $45K had higher success percentages, but the number of project with goal amounts that high was very low compared to the rest of the data, so it's better to look at the lower dollar amount campaign outcomes to determine chances of success based on dollar amounts.

<img width="576" alt="Play Outcomes Based on Goals" src="https://user-images.githubusercontent.com/106359572/174671908-58ccf20f-42d1-4602-b448-b7da1adef356.png">

### Challenges and Difficulties Encountered
It took an embarassingly long time to figure out that the reason my Outcomes vs Goals line graph did not look like the one shown in Canvas is because I was supposed to choose line with markers instead of stacked lines.

I did find several other formula errors though, while I was combing through the table to try and fix the chart (see highlighted ranges below that I had to correct several times to pull the right data.)  
The process for correcting my errors was repetetive and cumbersome because of the editing work that the formulas require (if I wanted to copy and paste, I had to choose whether to keep the highlighted ranges ).

<img width="914" alt="Outcomes based on Goals table" src="https://user-images.githubusercontent.com/106359572/174670385-5fe7624a-aedb-445c-a427-6f388dc06515.PNG">



## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
1. May is the busiest month
2. December is the slowest month.


- What can you conclude about the Outcomes based on Goals?
1. Success rates start high with lower goal amounts, and taper off to 20% once the goal amount reaches $25K.
2. There's another "sweet spot" of higher success rates for goals between $35K and $40K, but no goals higher than $45K were successful.

- What are some limitations of this dataset?
1. One limitation is that the data is several years old and similar data collected from post-covid times could look completely different, so I would be reluctant to make any decisions based on any of these analyses.

- What are some other possible tables and/or graphs that we could create?

1. We could create a pivot table with country as the main filter and parent category as another filter, to see what types of campaigns were most and least successful in each country.

2. We could filter again for only successful campaigns and calculate the total amount of money raised in each country, and then calculate the percentage of money raised vs. pledged to see which country had the highest percentage of goals achieved out of their pledges.
