# fantasy_ML_batters
## Problem
The problem we are looking to solve is in relation to fantasy baseball stats.
Knowing that we cannot perfectly predict the performance of any player at any given time, we would like to create a model to predict, with some accuracy, various metrics for an upcomming week, providing our team with an advantage over teams that rely on team managers to sift through upcomming matchups and past performance.

We would like to be able to provide a metric (R, H, HR, RBI, SB, BB, IBB, HBP, OPS) as a parameter, and in return get a predicted value for that player over the next 'X' amount of games.

If no metric is provided, we should receive predicted values for each of the 10 available parameters.

We will compare these values to the league averages to help determine whether this player would be considered an advantage or disadvantage of the upcomming week.

## Data Sources

All Data is being taken from https://www.baseball-reference.com/ and is being stored in local .csv files.

I've got full season stats for the past 5 seasons (2018-2022), with earilier season being weighted as less important that the most recent season.

There are also 2 more files: current season stats and last weeks stats. These will be the most heavily weighted data sets. 

The actual weight of each set is yet to be determined.

## Target Variable

I'm going to be predicting on of these 9 values (R, H, HR, RBI, SB, BB, IBB, HBP, OPS). All of these values are going to be able to be found in a StandardBatting data set (e.g 2022-BattingStandard), we are basing these predictions off of our advanced data (e.g 2022-BattingAdvanced). 




