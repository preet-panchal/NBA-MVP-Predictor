# PREDICTING NBA PLAYERS' PERFORMANCE 
(Repository: NBA-Star-Predictor)

## ABOUT US -----
* Hassan Chakaroun (Hassan-Chakaroun)
* .Mohammed (Mohammad0104)
* Preet Panchal (preet-panchal)
* Eihab Syed (EihabSyed)

We are Computer Science (Data Science Specialization) students at Ontario Tech University. We had the bright opportunity of learning multiple data science processes, methods and applications in CSCI2000U - Scientific Data Analysis course, led by Prof. Mariana Shimabukuro. As a group, we explore the "NBA Players" dataset and analyze it for potential data science applications. 

## INTRODUCTION -----

### The Topic: 
The National Basketball Association (NBA) is a professional basketball league in North America. The league is composed of 30 teams and is one of the four major professional sports leagues in the United States and Canada. It is the premier men's professional basketball league in the world. 

The selected dataset, “NBA Players” represents the data of NBA players from 1996-2020. We chose to study the topic of the NBA players because all of us are big fans of the game of basketball. Some of us also had dreams of playing in the NBA, but, here we are pursuing Computer Science. However, we have the amazing opportunity to study something we watch as fans on a daily basis. We are excited to present to you our findings and research about players in the league!

### Dataset Selected:
* Name: NBA Players Data - all_seasons.csv
* Source: https://www.kaggle.com/justinas/nba-players-data
* Reference: Cirtautas, J. (2021, August 2). NBA players. Kaggle. Retrieved November 26, 2021, from https://www.kaggle.com/justinas/nba-players-data. 
* Creator: Justinas Cirtautas, Data Scientist

### About the Dataset: 
The selected dataset contains over two decades of statistics referencing each player that was part of the NBA from 1996-2020. The data set contains over two decades of data on each player who has been part of an NBA teams' roster. It captures demographic variables such as age, height, weight and place of birth, biographical details like the team played for, draft year and round. In addition, it has basic box score statistics such as games played, average number of points, rebounds, assists, etc. In collection, the data set has 11700 rows and 22 columns each holding vast amounts of information pertaining to the NBA. If you want to learn more about how to improve the abilities and performance of NBA player, you're in for a treat! 

## DICUSSION -----

### Our Most Interesting Findings: 

#### How Weight and Height Affect Players' Performance? 
![This is an image]()
* From the scatter plot shown we can see a correlation of weight with points, players in the higher ranges of 140-160 kgs seem to have the higher points per game, where most of the players seem to have weights between 80-120 kgs. There does not seem to be a causation relationship but rather a correlation between average points and weight. We chose a scatter plot as it was the best option to easily view this specific data for users as it showed differences in points better.

![This is an image]()
* From the scatter plot shown we can see a correlation of height with points, players in the higher ranges of 210-230 cm seem to have the higher points per game, where most of the players seem to have heights between 190-210 cms. There does not seem to be a causation relationship but rather a correlation between average points and height. We chose a scatter plot as it was the best option to easily view this specific data for users as it showed differences in points better.

#### NBA All-Star Predictor: 
![This is an image]()
* To find the player with the most points, rebounds, assists, net rating, and shooting percentage respectively, of all-time our approach was to group by the player name and find the mean value of points, rebounds, assists, net rating, and shooting percentage. This allowed us to easily plot the data as a bar plot and found that the highest average points of all time was Lebron James with about 27 PPG (points per game), the highest average assists of all time was Chris Paul with about 9.5 APG (assists per game), the highest average rebounds of all time was Dennis Rodman with about 14 RPG (rebounds per game), the highest average net rating of all time was Jerrelle Benimon with about 120 points per season, the highest average team shooting percentage of all time was Jordan Sibert with about 1.5%. The challenge we faced for this task was to retrieve data that can be used in the mean() function, as originally the datasets values were a string type, in order to correct this during the data cleaning process we converted the data type of the values of age to integers using the astype() function for dataframes. We chose a bar plot as it allowed us to show the top 5 in each category easily.

### Was the First-round pick an NBA Bust? 
![This is an image]()
* To compare first-round, number-one player picks from each draft year with the most points, rebounds, assists, net rating, and shooting percentage respectively, our approach was to use boolean indexing to filter out for players whose draft number is 1 and then group by the player name and find the mean value of points, rebounds, assists, net rating, and shooting percentage. This allowed us to easily plot the data as a bar plot and found that the highest average points of first overall players was Lebron James with about 27 PPG (points per game), the highest average assists of first overall players was John Wall with about 9 APG (assists per game), the highest average rebounds of first overall players was Dwight Howard with a little under 12 RPG (rebounds per game, the highest average net rating of first overall players was David Robinson with about 10 points per game, the highest average team shooting percentage of first overall players was Zion Williamson with about 0.7%. The challenge we faced for this task was to filter out players who were first overall draft picks and to retrieve data that can be used in the mean() function, as originally the datasets values were a string type, in order to correct this during the data cleaning process we converted the data type of the values of age to integers using the astype() function for dataframes. This data will also be useful later on for potential data science applications, as we will see in one of our confusion matrices.

#### Predicting NBA All-Star Players: 
![This is an image]()
* Our model’s results were based on using 25% (584 players out of 2333 players, 162 players were All-Stars, and 2171 players weren't All-Stars, total: 2333) of unique players. Based on the results of our model, we see that our All-Star class has a precision 98% and our Not All-Star class has a precision of 85% which shows that our model is fairly precise when it comes to predicting true All-Stars as its precision is 98%, and is also fairly decent when predicting true Not All-Stars as its precision is 85%.
Likewise, the value of recall for our All-Star class is 99% and for our Not All-Star class is 75% which shows that our model can prevent mistakes when predicting true All-Stars but has mistakes when predicting Not All-Star as All-Star, we can view this false positive as our predictor indicating that this player has the potential to become and ALL-Stars. The accuracy of the model on the data set is 97%. Since precision for All-Star was very high and recall for Not All-Star was also high, using an f1-score would be ideal to accurately measure our models performance. Based on the f1-score of our model, 98% of all All-Star were predicted correctly and likewise 80% of Not All-Stars. This leads us to believe that 20% of players that are not currently All-Stars have the underlying numbers to become an All-Star. 
The mean average of precision was 91% and the mean average of recall was 87%. The weighted averages represent the sum of the scores of all classes after multiplying their respective class proportions.

## CONCLUSION -----

As a group, we learned many things from the “NBA Players” dataset. We believe that our findings and analysis of this dataset can be extended for the use of coaching and development staff in the NBA league. Our research can be used to determine if factors such as height and weight affect the player's performance. The NBA teams’ training and development staff can help improve particular players using this research. Furthermore, the NBA teams can also see statistics of which college or country the best players come from, so they can draft the best of the best for their team. 

#### Reflection:
Many lessons were learned in this course and also in this final project. With the “NBA Players” dataset, our group’s biggest downfall was figuring out how to build a successful confusion matrix for machine learning applications with this dataset. We did not see potential for comparing existing columns within the dataset, thus, we decided to generate our own variables (ex. All-star player) to build important connections, correlations and findings using the confusion matrix, in order to conclude valuable potential data science applications. 
