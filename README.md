# Kickstarter Analysis Challenge

## Overview of Project

In this project, I aim to conduct a series of analyses and visualizations using Microsoft Excel on a Kickstarter projects dataset. The dataset includes project-specific data such as its name, blurb, goal, pledged funding, outcome, campaign launch date and deadline, category, etc., of various projects in different countries, which can be employed to inform new Kickstarter projects on how to plan for their fundraising campaigns.

### Purpose

To help Lousie, an up-and-coming playwright, decide on setting a smart fundraising goal for her new play entitled "Fever," and specifcy the optimum timing for launching her campaign.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

![This is an image](/Theater_Outcomes_vs_Launch.png)

In this part of the analysis, in a sheet named "Theater Outcomes by Launch Date," I tried to figure out what month of the year is the best time for Lousie to launch her fundraising campaign. For this purpose, I created a pivot table in a separate sheet representing the outcome of projects given the month they were started. Since Louise's play is categorized under the "Theater" parent category, I filtered the table by "Theater" and narrowed the results to a more relevant subset of data. Then, using a pivot chart (Line with Markers), I revealed the latent trend within the data, vis a vis, the outcome of projects based on launch month. As shown above, while the number of successful projects weakly fluctuates from January to April (between 56 to 71), this number reaches its highest value in May (111). However, afterward, the number decreased gradually to its pre-May level by November (54 successful projects) and even a lower level in December (37). The failed project monthly trend somehow shows the same pattern except that the number of failed projects does not increase sharply in May and remains almost constact for the three following months. Finally, the number of canceled projects remains virtually the same during the year as they comprise a small portion of the total projects (the number of canceled projects every month is less than 10). These results indicate that the largest number of successful projects were launched from May to July (maximum number in May with 111 successful projects).

### Analysis of Outcomes Based on Goals

![This is an image](/Outcomes_vs_Goals.png)

In the second part of the analysis, in a new sheet named "Outcomes Based on Goals," I tabulated project goals (split stepwise) against the number and percentage of projects with successful, failed, or canceled outcomes. Using "COUNTIFS" and "SUM" functions, I could obtain the number of projects for each outcome type given the range (less than 1000, equal or more than 1000 to 4999, equal or more than 5000 to 9999, ..., more than 50000) in which project goals reside. This allowed me to calculate the total number of projects for each goal range and, consequently, the percentage of projects for each outcome type. Using the obtained values, I then created a line chart by which the percentage of success, failure, and cancelation can be traced throughout the specified goal ranges. The trends indicate that project success was more than twice compared to failure when the project goal was set to less than 1000. However, this success prevalence ratio diminishes as the set goal increases to between 15000 and 19999 (equal success and failure rate). This trend persisted so long as the projects remained more likely to fail for goals from 20000 to 34999. However, surprisingly, projects with higher goals of between 35000 to 44999 became more successful. This pattern, nonetheless, retreats to absolute failure (%100 failure) for goals from 45000 to 49999 and almost failure (%88 failure chance) for goals above 50000.

### Challenges and Difficulties Encountered

Fortunately, I did not encounter major challenges or difficulties during the entire analysis process. The only part I might have needed help with working with Excel was the data format conversion for the Unix datestamps, which, hopefully, I could resolve following the instructions. I also can mention a difficulty I experienced when adding the screenshots to the Readme file. With the help of the TA, I could figure out that file names with spaces included will not be rendered for visual display. Overall, I think the guidance and explanations offered were more than enough to fulfill the tasks, and the additional resources were very helpful for resolving any unexplained concepts.

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

Overall, theatre projects can be considered reasonably successful, and the number of successful projects outweighs the number of failed projects throughout the year.
Month May (also June and July to a lesser extent) looks an excellent timing for Louise to launch her campaign (Although the success rate for each month may also be a worthy indicator for choosing the timing of the campaign, given the almost similar number of failed projects for a different month, the number of successful projects can be realized as an appropriate indicator in this case).

- What can you conclude about the Outcomes based on Goals?

Given the results, setting goals less than 15000 and between 35000 and 44999 would be wise for Lousie as projects in these goal ranges were more likey succeed. However, given the low number of projects (which may not be reliable) in the later range and minute discrepancies between success and failure for goals from 5000 to 14999, I believe it would be optimal if Lousie set a goal up to 5000.

- What are some limitations of this dataset?

The initial dataset did not distinguish between categories and subcategories, which was required for further scrutiny.
Another issue was the currency types and values. In this dataset, there is no distinction between currency values. For a more realistic comparison, an estimation of currency conversion rates should be added to make necessary adjustments.
Although the number of backers is helpful in assessing the viability of the projects, the within-backers variations (gender, wealth, nationality, job, etc.) could also help further our analysis.

- What are some other possible tables and/or graphs that we could create?

There were plenty of other options to use to visualize our results. For example:
Pie charts could be used to better display the share of numberical values (for example, the percentage of successful projects).
One could use histograms to examine the distribusion of numerical variables for potential statistical tests.
Bar charts could be used for comparisons between categorical variables such as outcome or country.
Scatterplots could also be used to identify relationships between numerical variables (for example, pledged and campaign length).
