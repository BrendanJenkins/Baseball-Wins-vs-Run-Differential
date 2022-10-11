# Baseball-Wins-vs-Run-Differential
## Introduction
In the early 2000's there was flawed perception about what led to wins. Many orginizations thought they just needed more star power to get more wins, so they would compete to see who could spend the most money for star players. This led the teams with smaller payrolls to ask how they could compete with these rich teams while spending less money. This led to the analytics revolution in baseball. When analytics hit baseball, one of the first research questions was "What creates a win?". In this repo I explore this question.

## Data
The data for this repo comes from [Sean Lahman's Databank](https://www.seanlahman.com/baseball-archive/statistics/). Specifically, I used the Teams.csv file which has the final stats for each team from each season.

## Techniques
The main technique I used for this was Linear and Lasso Regression. I specifically chose these two models because I wanted to have an interpretable model. One thing that really stood out to me was the nearly perfect linear relationship Run Differential has with Wins. A Run Differential of 0 leads to 81 expected wins, which is exactly half of the 162 game season. The beta coefficient for Run Differential was roughly 0.1, which means for every 10 runs a team scores above the amount they give up, they could expect to win 1 more game. So, if a team is looking to get to the 95 win mark, the average number of wins for a team that makes the playoffs, then they should work to have a run diffential of +140 or more.
