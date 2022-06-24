# Kickstarting with Excel

## Overview of Project

The following analysis is meant to examine the relationships in crowd funding for theatrical plays. We will review data behind a variety of kickstarter crowd funding projects determine what made some efforts successful, and what pitfalls should be potentially avoided in order to reduce the odds of failure. 

### Purpose

The specific purpose of this analysis is to provide users of this information guidance on how to interpret the data from previous kickstarter endeavors. The goal is to take the data and create a meaningful interpretation that builds upon the raw data into something that sheds light on the important variables to consider in launching a kickstarter campaign.

## Analysis and Challenges

I performed analysis of the data in the kickstarter_challenge file by evaluating the tables correlating outcomes of kickstarter campaigns with the months that campaigns were launched and the original funding goals. One of the initial challenges with this module was creating the tables to correlate the data correctly. The analysis relies on accurate association of goals to outcomes. Another challenge, and probably more of a qualitative one, was to consider the population of outcomes in each bracket. Viable analysis can really only be trusted if there is a robust dataset with ample sample size to draw logical conclusions. In some of the correlation brackets of campaign goals to outcomes, the sample sizes are so small that the outcome analysis might be more suspect. 

### Analysis of Outcomes Based on Launch Date

An initial glimpse at the data and corresponding visualization indicates that the best time of year to launch a funding campaign is May, with a seemingly linear regression throughout the following months until around September when things bottom out. The outcomes of campaigns in May and through the "summer" months seem so outstandingly superior that further analysis might initially seem superfluous. But a deeper look must take into consideration the sample size for each period. 
<p align="center">
  <img src="https://github.com/cb19weber/kickstarter-analysis/blob/main/resources/Theater_Outcomes_vs_Launch.png" />
</p>
But a deeper look must take into consideration the sample size for each period. May and June, respectively, have the most and second-most successful outcomes when correlated to launch date. But they also have the greatest amount of failures. There were more campaigns launched in these months than in other months, and so correlating the outcomes to the launch dates is more complicated than just choosing the month with the greatest successful outcomes. The gap between successful and failed outcomes by periodic launch date might give more relevant information. The greater quantitative difference between successful and failed campaigns depicts the success rate of those kickstarters. This validates that campaigns launched in May have the best odds of success. The success rate steadily declines after May until December when it is almost a 50/50 chance. Outside of December, the launch outcomes by period are actually closer than what initial evaluation might suggest, with most periods having a success rate around sixty to just under seventy percent. The conclusions to draw here are 1) don't launch a kickstarter campgain in December, and 2) the summer months may offer slightly higher odds of campaign success, but the outcomes will likely be on other variables.

### Analysis of Outcomes Based on Goals

This analysis examined another potential variable correlation to kickstarter success by comparing outcomes based on the initial goals of the campain. The initial glimpse of the data and associated visualization here looks like things might be all over the map. But the sample size of campaigns with goal exceeding $10,000 is extremely limited. Exactly how limited? There were fewer kickstarter with goals exceeding $10,000 than there were in any of the smallest three goal buckets analyzed. So while it looks like things are all over the map, if the data were evaluated based simply on having an "over $10,000" bucket to capture all higher goal campaigns, there is a clear linear relationship between smaller fundraising goal and success rate.
<p align="center">
  <img src="https://github.com/cb19weber/kickstarter-analysis/blob/main/resources/Outcomes_vs_Goals.png" width="65%" />
</p>
The conclusion here is actually more of a challenge to potential playwrites and their dream of successfully funding their play. Keep your budget as tight for a real shot at meeting fundraising goals.

### Challenges and Difficulties Encountered

I think some of the challenges of this dataset have already been highlighted in some of the analysis provided above, but two of the largest challenges worth mentioning here is the type of line graph that was chosen to visualize the outcomes against the launch dates and the expansive table selected to analyze the outcomes against various goal ranges. The visualization of the outcomes based on launch date makes it look like May and June are very clear winners for when to launch a campaign. When you actually evaluate the success rate, the difference between most months other than December is actually quite small, with the average being just around 62%. Additionally the definition and breakouts of the various goal ranges for the outcomes based on goals chart creates a visual that looks very disjointed. In reality, there are so few campaigns with goals greater than $10,000 that they really should all be grouped together rather than evaluated separately. When the table is altered this way, the success rate of campaigns exceeding $10,000 is only 46% and creates a much more reasonable visualization.

## Results

I think the result of this analysis and module is really getting used to looking at your dataset and understanding it a bit before choosing how to organize and visualize the data. Chart visualizations can be extremely informational, but they can also be very misleading if based on information that isn't relevant or is heavily skewed by outliers.
