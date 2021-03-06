# NBA-Projcet
Estimating PPG for top 500 NBA players of all time

Question of Thesis & Motivation for Research

For this project, I will be analyzing a data set of the “Greatest 500 NBA Players of All Time” in order to
find the best predictors for PTS, career average points per game. When ranking players in the NBA, the first
variable of importance that comes to mind would likely be Points, as those who are viewed as the best players
are often the ones who get a lot of points per game. I hope that by analyzing the relationship between PTS
and the other variables in the data set, such as Minutes Played and Shooting Percentage, I will be able to
better determine what makes a “great” player.

First off, I will estimate what I think will be the best predictors, and create a linear model containing them
as predictors for PTS. Then, my approach to finding the best set of predictors will start by creating a “Full
model,” in which PTS will be estimated through a covariance adjusted model with all of the other variables
in the data set used as predictors. After this, I will create a “Reduced Model,” removing the predictors that
were not significant in the “Full Model.” Then, I will use Akaike Information Criterion (AIC) to select a
model. This method of selection creates many models, and then compares them to the full model. The best
model is determined as the one with the lowest AIC score. AIC variable selection also requires the data
to have no missing values, so this model will show how the 3 point line changed scoring. Last, I will use
Bayesian Information Criterion (BIC) to select a model, which is similar to AIC, but prefers smaller models.

The data was downloaded on November 2 2017. This is worth noting, as there are some active players on this list, whose stats will change slightly throughout the season. The original data set has 16 variables for 500 NBA players. The variable are:

Rank    
Player Name
From   -   The year the player's career started

To     -   The year the player's career ended

G      -   Total games played in career

MP     -   Career average minutes played per game

PTS    -   Career average points per game

TRB    -   Career average total rebounds per game

AST    -   Career average assists per game

STL    -   Career average steals per game

BLK    -   Career average blocks per game

FGpct  -   Career average field goal percentage

3Ppct  -   Career average three point percentage

FTpct  -   Career average free throw percentage

WS     -   Win Shares (An estimate of the number of wins contributed by a player)

WS/48  -   Win Shares per 48 Minutes (An estimate of the number of wins contributed by a player per 48 minutes)
