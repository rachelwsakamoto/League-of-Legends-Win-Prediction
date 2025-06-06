---
title: League-of-Legends-Win-Prediction
date: June 6, 2025
---

<h1> League of Legends Prediction </h1>

<h2> Introduction </h2>
<p> League of Legends is a very popular game amongst the younger generation. The top percentile of playes can even make a living off of being good at the game. Naturally, if there is a pattern that can be observed that brings in more wins, we would want to find that out. Is there any pattern between those that choose Ashe versus Caitlyn as their Champion? </p>
<p> There are 5 rows in this dataset. We will be exploring the columns 'champion' (tells us the name of the fighter that the user plays as), 'results' (tells us if the game is won or last 1 being a win and 0 being a loss), 'kills', (tells us how many kills the player received per game) </p>

<h2> Data Cleaning and Exploratory Data Analysis </h2>

<p> I cleaned the data by filling empty values in the 'kill' column with 0. By doing so, I am able to make use of the data and later be able to make a prediction of it. I chose to replace empty values with 0 becasue it is a plausible replacement as some users may have left the game early, leading to this value. Because it is a fair replacement, this should not construe the data far from the truth.</p>

<img src="bivariateanalysis.png">
<p> This plot shows the relationship between the number of games a user plays and the numbers of kills they get per game if they choose Cailtyn as their champion. It appears that the less number of games played, the more kills they may have gotten </p>

<img src = "interestingaggregate.png">
<p> This table is grouped by users that chose Ashe and users that chose Caitlyn as their champion and by their result. This may give us a general idea of what our conclusion may look like. 

<h2> Assessment of Missingness </h2>
<p> I do believe that the 'damagetakenperminute' column is NMAR. We tested the 'damagetakenperminute' column to see if it is affected by other columns. To do this, we ran permutation tests to including the 'gamelength' column and the 'side' columnn. Those that tended to play a longer game had higher values in their 'damagetakenperminute'.

<p> not done </p>

<h2> Hypothesis Testing </h2>

<p> Null Hypothesis: Ashe and Caitlyn have the same average kills per game</p>
<p> Alternative Hypothesis: Ashe and Caitlyn do not have the same average kills per game </p>
<p> Test Statistic: Permutation Test</p>
<p> Significance level: 0.05 </p>
<p> p-value: 0.0610 </p>
<p> I chose a permutation test because the distribution may be skewed because there are many different people that play this game, so normality is not guranteed. Permutation tests work for any sample size and distribution, so I thought it would be much safer to run a permutation test rather than a hypothesis test that has a lot of restrictions. </p>

<h2> Framing a Prediction Problem </h2>

<h2> Baseline Model </h2>

<h2> Final Model </h2>

<h2> Fairness Analysis </h2>