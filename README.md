# An Analysis of Kickstarter Campaigns.
Performing analysis on Kickstarter data to uncover trends

## Overview of Project

To discover how successful different campaigns were, based on their launch date and pledge goal.

### Purpose

This will help Louise determine the best options for her next campaign.

## Analysis and Challenges
### Analysis of Outcomes Based on Launch Date

Using a pivot table, I was able to filter the data I needed to see how launch date affected the success rate of campaigns. This can be found on the Wooksheet "Theatre Outcomes by Launch Date". The biggest challenge was determining how to make the rows be months, but this was solved by getting rid of the "years" and "quarters" fields. I was then able to chart this out.

![Theatre_Outcomes_vs_Launch](https://user-images.githubusercontent.com/103209236/164543856-674339c7-0f3e-4621-969a-4caf589863fa.png)

### Analysis of Outcomes Based on Goals

To get the success rate of plays by pledge goal, I created a new table in the worksheet "Outcome Based on Goals". Separating the goal amounts by every $5,000 was a great way to oranize the data, but I wasn't sure how to get the amount of successful or failed for each goal. COUNTIFS() proved useful. For each column I would use COUNTIFS() to filter the goal amount between two points, the outcome (successful, failed, or canceled), and made sure I was only getting data for plays. After getting the number of each outcome, I added them up and divided to get the percentage for each one. I was then able to chart it out.

![Outcomes_vs_Goals](https://user-images.githubusercontent.com/103209236/164545295-a5875df4-5d2d-43db-94af-6ed0dc9d9f64.png)

## Results

To help Louise determine perameters for her next campaign, I've discovered several things...

1) In "Theatre Outcomes by Launch Date", the best time to start a campaign is in May (June and July are also solid choices)
2) In "Theatre Outcomes by Launch Date", the worst time to start a campaign is December, with almost as many failed campgains as successful ones.
3) In "Outcomes Based on Goals", it's best to have a low pledge goal, around $5,000 or less. While there were a large percentage of successful goals in the $35,000 - $45,000 range, there were only 9 campaigns launched so there isn't enough data to support this. 

All in all, the data points to launching a campaign for around $5,000 in May. 

For a more in depth view, I could have filtered countries to see if different ones had different outcomes. I could have also used the amount of backers/average donation to see if smaller campaigns rely on having 1 or 2 large backers. The data is also missing some points that could have helped see a bigger picture. How well known are the people working on the projects? How much money/time/effort is put into fundraising and marketing for the the campaign? While many campaigns are in the US, how many were in LA vs NYC vs elsewhere?

While the questions could have helped Louise, I feel confident in my findings.

>‘Brevity is the soul of wit.‘
(Hamlet, Act 2, Scene 2)
