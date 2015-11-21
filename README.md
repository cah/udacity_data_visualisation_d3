#Udacity Data Analyst Nanodegreee
##Data Visualization and D3 Project

###Summary

A data set containing 1,157 baseball players including their handedness (right or left handed), height (in inches), weight (in pounds), batting average, and home runs. The visualizations should communicate the edge that left handed baseball players have in batting average and Homeruns.

#####The dataset is available:
https://www.google.com/url?q=https://s3.amazonaws.com/udacity-hosted-downloads/ud507/baseball_data.csv&sa=D&usg=AFQjCNEjepW24JPVyIpheLuF7wHlFJd2rg


#####Dataset columns:

1. name      : Players Name 
2. handedness: Left Handed, Right Handed, or Both (Switch Hitter)
3. height    : Player Height 
4. weight    : Player Weight 
5. avg       : Batting Average 
6. HR        : Number of Homeruns

###Design:

1. Remove Players with zero batting average and zero homeruns 
2. Since handedness is categorically data, I selected a bar chart 
3. Provided read two charts: batting average and homeruns by handedness

###Feedback:
1. Version One Feedback
  1. Chart Needs Title
  2. Needs title cleanup on x
  3. Needs title cleanup on y
  4. Weight on x axis is too busy
  5. Consider moving legend 

2. Version Two Feedback
  1. Legend needs title
  2. Would be helpful to filter on handedness

3. Version Three Feedback (provided by Udicaty Coach)
  It looks like this visualization is plotting the total home runs within each weight bin. The problem with plotting total home runs is that a bin with more players is probably going to have more total home runs. That really only tells me as chart reader that 190 weight bin has the most players in it. The chart also implies that there are mostly right handed players in the data set, then left handed players, and finally switch hitters. But that isn't a relationship between handedness, home runs, and weight; instead, it is indirectly showing the counts of players within each weight bin like a histogram. This makes the plot more exploratory rather than having a clear explanatory story.

One possible solution is to find the average number of home runs within each weight bin. That would be the total home runs divided by the number of players within each bin. But, I can't guarantee that this will show an interesting correlation or relationship. It might not, so more exploratory data analysis will have to be done to find an explanatory story.

Questions that might lead to an explanatory story:

are home runs and batting average correlated?
do right handed players tend to have better performance statistics than left handed players?
do heavier and/or taller players score more home runs or have better batting averages? Or does BMI (http://extoxnet.orst.edu/faqs/dietcancer/web2/twohowto.html) correlate to batting player performance?
One side note: this data set contains quite a few players with a batting average of 0. It's likely these were pitchers who had designated hitters https://en.wikipedia.org/wiki/Designated_hitter . It might be better to remove these points before doing analysis on baseball player performance.


###Resources:

1. http://d3js.org
2. http://dimplejs.org/examples_viewer.html?id=bars_vertical_stacked
3. http://dimplejs.org/advanced_examples_viewer.html?id=advanced_interactive_legends
4. http://dimplejs.org
5. https://www.udacity.com
