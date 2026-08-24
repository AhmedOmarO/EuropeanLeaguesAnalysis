# European Football: Player Performance Across Age

An exploratory analysis of how professional football players' performance changes with age, using the European Soccer Database covering matches and player attributes from 2008–2016.

## Question

**At what ages do football players tend to perform above or below their career average?**

Player rating is used as a proxy for performance. For each observation, the analysis compares a player's rating with that player's own average, then aggregates the percentage difference by age. This within-player normalization makes the age pattern easier to interpret across players with different baseline ability.

## Key finding

![Average player rating change by age](Key%20Finding.png)

Players performed most strongly between approximately ages 24 and 32, with ratings averaging about 2.5% above their individual career means.

## Approach

- Load and inspect the European Soccer Database
- Clean and join player and player-attribute records
- Calculate each player's average rating
- Express individual observations as a percentage difference from that baseline
- Aggregate and visualize the relationship between age and relative performance

## Repository contents

- [Analysis notebook](Players%20rating%20change%20with%20age.ipynb)
- Supporting data and exported visualization

## Tools

Python, pandas, NumPy, Matplotlib, Seaborn, SQLite, and Jupyter Notebook.

## Context and limitations

This project was created as part of the Udacity Advanced Data Analysis Nanodegree. Ratings are an imperfect proxy for real-world performance, the data ends in 2016, and the analysis is descriptive rather than causal.

## Further work

A useful extension would be a player-level forecasting tool that estimates which attributes are likely to improve or decline based on current age, position, rating, and historical development patterns.
