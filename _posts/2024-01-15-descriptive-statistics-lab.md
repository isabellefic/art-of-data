---
layout: post
title: Descriptive Statistics - Baseball
subtitle: Lab 3
cover-img: /assets/img/lab3/BaseballBackground.jpg
thumbnail-img: /assets/img/BaseballLogo.png
tags: [baseball,labs]
---

I worked with a dataset about MLB baseball teams. The dataset shows a lot of stats about the batting and fielding performances by each team during each season from 1876 to 2020. I chose to work with this dataset because the season is quickly approaching and I am looking forward to watching!

I am interested in looking at the statistics of world series winners vs non-world series winners to see what strengths a team needs to have to be able to advance to the World Series, specifically the Yankees :).

The first factor that I thought might influence a team’s chances at the world series is the # of home runs that they score in a season. However, since the dataset includes teams from the 19th century where they were playing only between 60 and 100 games per season (compared to the 162 games per season now), I calculated the number of home runs per game instead of just plotting the number of home runs which would result in a much larger range of data and could drag down the mean and median of both the world series and non-world series winners. Despite the consideration for the fewer games in earlier seasons, these graphs look pretty similar. The number of home runs per game is only slightly higher in world series winners compared to non-world series winners.
![Graph1](https://isabellefic.github.io/art-of-data/assets/img/lab3/1.png)

Once I saw that these graphs were very similar, I thought about factors that could be increasing the number of home runs per game for the non-world series winners. One factor that came to mind was that playoff teams that were still very good were counted in the non-world series winners. To repair this issue, I made graphs for both playoff and non playoff teams instead of world series winners. These graphs showed that playoff teams were scoring slightly more home runs with a median of 0.93 compared to a median of 0.90.
![Graph2](https://isabellefic.github.io/art-of-data/assets/img/lab3/2.png)
![Graph3](https://isabellefic.github.io/art-of-data/assets/img/lab3/3.png)

However, home runs scored could not be the sole reason for a strong performing team; so, I decided to create a similar pair of graphs of the number of hits per game to see if that had a larger impact on world series winners. These graphs showed a larger difference between world series winners and non-world series winners. The median hits per game is 9.21 in series winners and 8.83 in non-series winners.
![Graph4](https://isabellefic.github.io/art-of-data/assets/img/lab3/4.png)

I also calculated the on-base percentage of each team, which is the number of times they got on base divided by the number of at-bats. I then calculated the slugging percentage, which is the total number of bases per at-bat. After I had the on-base percentage and the slugging percentage, I added them together to get the OPS (OBS + slugging). After I had calculated the OPS, I graphed that against the number of runs scored and saw a strong relation between the two variables.
![Graph5](https://isabellefic.github.io/art-of-data/assets/img/lab3/5.png)
I also noticed that there were a few outliers in this graph which certainly affected the correlation, which was only 0.71. Aside from those outliers, there was a strong visible correlation between these two variables.

I also plotted a histogram of the hits per game to see the shape of the distribution of the graph and it looks fairly normal.
![Graph6](https://isabellefic.github.io/art-of-data/assets/img/lab3/6.png)
There are a few data points that lie to the right of the main curve so the data is slightly skewed right; however, it is a mostly normal distribution.

One limitation of this dataset is the fact that some of the data from the early years of the MLB is missing. They did not have a world series or divisions, and they did not record stolen bases, sacrifice flies, and other pieces of information.

Finally, one more simple graph that I plotted was a graph exclusively of world series winners. I graphed the number of the world series winners that were also the winner of their division.
![Graph7](https://isabellefic.github.io/art-of-data/assets/img/lab3/7.png)

From this graph I learned that for the New York Yankees to have the highest chance of winning the world series, they need to win their division first. 😀
