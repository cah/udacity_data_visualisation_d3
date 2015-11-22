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
#### Version One
##### Feedback
1. Chart Needs Title
2. Needs title cleanup on x
3. Needs title cleanup on y
4. Weight on x axis is too busy
5. Consider moving legend 

##### Modifications
1. Added Title 
2. Provided more specific Title on x and y 
3. Rounded Weight to ensure chart was easier to understand
4. Moved legend to ensure read is able to find it

#### Version Two 
##### Feedback
1. Legend needs title
2. Would be helpful to filter on handedness

##### Modifications
1. Added Legend Title
2. Added Filter by handedness 

#### Version Three 
##### Feedback (provided by Udacity Coach)
 1. It looks like this visualization is plotting the total home runs within each weight bin. The problem with plotting total home runs is that a bin with more players is probably going to have more total home runs. That really only tells me as chart reader that 190 weight bin has the most players in it. The chart also implies that there are mostly right handed players in the data set, then left handed players, and finally switch hitters. But that isn't a relationship between handedness, home runs, and weight; instead, it is indirectly showing the counts of players within each weight bin like a histogram. This makes the plot more exploratory rather than having a clear explanatory story.  One possible solution is to find the average number of home runs within each weight bin. That would be the total home runs divided by the number of players within each bin. But, I can't guarantee that this will show an interesting correlation or relationship. It might not, so more exploratory data analysis will have to be done to find an explanatory story.  

##### Modifications
1. Shifted charts to be explanatory

#### Version Four
##### Feedback (provided by Udacity Coach)
1. replace a little bit cryptic R, L and B in charts with full Left, Right and Both labels.
2. consider using single color for all bars, except Left. It will highlight its uniqueness even more. Try light gray for Right and Both and some more bright color for left.

##### Modifications
1. Replaced labels on x axis with Left, Right and Both (replaced L,R,B in the csv file)
2. Used grey for Right and Both ensuring the reader would focus on the Left bar
 
###Resources:

1. http://d3js.org
2. http://dimplejs.org/examples_viewer.html?id=bars_vertical_stacked
3. http://dimplejs.org/advanced_examples_viewer.html?id=advanced_interactive_legends
4. http://dimplejs.org
5. https://www.udacity.com
