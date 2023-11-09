# LHL-Capstone-Project

## Project/Goals
This capstone will focus on the analysis of the Raptors / Cavaliers seasons, and also looking into the star players if they had any affect during the playoffs. The goal of this project is to find out the reasons why Raptors have been losing to the Cavaliers for three seasons straight in the playoffs, and how to overcome these losses. I'll also be comparing the star players on each team to see who's consistently performing well and whos playing below average compared to the regular season. The insights from this analysis could significantly influence both team strategy and player development in several ways such as strategic adjustments, player conditioning, targeted skill development, tactical game plans, roster management, and opposition analysis.

## Process
Problem: 
Seasons 2015/2016/2017 Raptors have been struggling consistently against the Cavaliers during the playoffs.

Hypothesis: 

Raptors are severely underperforming in the playoffs due to the pressure and stress. The pressure is a lot higher on the star players such as Kyle Lowry and DeMar Derozan thus causing the team rhythm to drop. Also, when the Raptors are not playing in home territory, it gets alot worse, especially on their defense. Teams would most likely score alot higher in the playoffs compared to the regular season against the Raptors during away games.

Collect Data:
 
The data was collected from "balldontlie.io" API, website had organized endpoints which made collecting data alot easier. Endpoints such as Get ALL Stats, Get All Games, and Get All players were used to retrieve the information.

Cleaning: 

All codes and data cleaning were performed on VS Code while using Jupyter Labs and Pandas. First thing I noticed for all files was that there were a high amount of rows for a filter of just three seasons. Before I checked for duplicates, the data types were also checked. Date column came as object, converted it to datetime format and organized the dataframe according to the date. Duplicated rows were checked on all dataframes and they all came back with high amounts of duplicates. Once removed, nulls/nans were then looked at, some dataframes came back with none, while others came back with high amounts (players missing games and getting no stats for that particular game), blank rows were also checked with no findings across all dataframes. Lastly, unnecessary columns were removed. Outliers were visualized on VS Code, due to each stat affecting a players total average (outliers were not removed). Sport analyzation for outliers must remain to get an accurate average for the individual player. Sometimes a player might score exceptionally high and removing that outlier will decrease the players average.

Analysis of Data: 

The dataframe for both the Cavaliers and Raptors did not track the wins or losses of each game, I made a new column called Outcome to solve this issue. Also, I made a Latitude and Longitude column for home team columns so that I can later visualize where the Raptors were losing on a map in Tableau (Note: cities had odd names in the dataframe such as Goldenstate, the coordinates would make it easier within Tableau). I found that the Raptors' stats dataframe was unusable due to off numbers, a 75% lack of dates, and distorted visualizations, in contrast to the Cavaliers' stats dataframe. Whole dataframe was unusable compared to the Cavaliers stats, same code was applied to retrieve data from the API, but it was a lot more accurate. 

The following statistical and analytical methods were utilized:
1. Descriptive statistics: Basic statistical measures such as mean, median, and mode were used to summarize the central tendency of the players performance metrics

2. Data Visualization: Matplotlib, Seaborn, and Tableau were used

3. Trend Analysis: This method was employed to identify patterns over the three seasons, particularly looking at how performance metrics changed from the regular season to the playoffs.

4. Comparative Analysis: Head-to-head comparisons between players (e.g., Lowry vs. Irving, DeRozan vs. James) were made to assess relative performance levels.

5. Correlation Analysis: To explore relationships between variables, such as the impact of home versus away games on performance and the correlation between regular-season success and postseason outcomes.

6. Outlier Analysis: Instead of removing outliers, they were examined to understand their impact on the players' average performance, providing a more nuanced view of player capabilities during exceptional games.



ChatGPT
There are several spelling and grammatical issues in the text provided. Here's a corrected version:

Do Raptors compete a lot harder during home games, and how well do they play in the playoffs compared to the offseason? A map (Away Games) and bar graph (Home Games) were used in Tableau to show which cities Toronto has defeated during the regular season. The Raptors struggled a lot more in the Western Conference compared to the East. What I noticed was that Toronto struggled severely during away games, especially against the Cavaliers in Cleveland. The Raptors had a lot more wins (166-80 W/L) compared to the Cavaliers (158-88 W/L), but in the playoffs, they would perform severely low (18/24 W/L). This indicates they are not playing up to par in the playoffs, likely due to stress and pressure. They should not perform this low against teams they have beaten in the regular season with ease. A bar chart was used to visualize both postseason and regular season. Lastly, two pie charts were placed to show the number of points Toronto scored against opponents in the playoffs. One pie chart shows the home games and the other, away games. This gave us an understanding of the number of points they would score during home or away games, and unsurprisingly, Toronto would produce fewer points during away games by a huge average of 11 points.

Where do the Cavaliers face their toughest challenges, and which teams serve as a benchmark for their offseason analysis? Like the first dashboard in Tableau, I placed a map representing the away games and a bar graph representing the home games. I only focused on the losses for the Cavaliers to see which teams gave them the most trouble during home and away games. In home games, the Cavs face tough competition from teams like Washington, Atlanta, and Chicago. These teams have consistently outperformed the Cavs, and they offer valuable lessons on defense and court strategy. Away games present an even bigger challenge, particularly against teams like Miami, as highlighted by the included bar chart where the margin is considerable. Lastly, two pie charts were shown just like the first dashboard but with Cleveland now. The Cavs would score a lot higher against the Raptors during home games compared to an away game, and this is a difference of about 8 points.

How does Kyle Lowry's season-long performance hold up, especially when the playoffs heat up? Three bar graphs were placed to show Kyle Lowry's season averages, playoffs against Cleveland in an away game, and playoffs against Cleveland during a home game. Surprisingly, he performed quite well compared to my hypothesis. I thought he would play a lot worse during away games, but he averaged almost the same amount during the regular season. One thing caught my eye: Kyle Lowry's assists were a lot higher during away games, and his points almost equaled his season average. I also placed a bar chart showing his opponent, Kyrie Irving, and what he averages during the regular season. When we compare these numbers, we notice that Lowry holds his ground well, suggesting that while there are areas to improve, he's not the sole factor in playoff outcomes.

How well does DeMar DeRozan play under pressure during away games in the playoffs? Similar to Kyle Lowry's dashboard, bar graphs were used, and instead of Kyrie, this time LeBron James was used as a comparison. To start off, we see a player who shines in home games, with a noticeable difference in performance when he's on familiar ground. In playoff games, particularly at home with an average of 27 points, DeRozan's stats are solid. However, his performance in away games, especially against LeBron James, shows a need for strategic adjustments. The numbers drop to an average of 14 points, which is a huge loss for the Raptors, especially in an away game where every point matters. Comparing DeRozan to LeBron, we see that DeRozan holds his own at home but struggles to match LeBron's impact in away games, highlighting an area for focus in training.

How much of an insight do the Cavaliers' stats give us? Four bar graphs were shown to give us an understanding of the Cavs' team. The averages of the entire team (points, assists, blocks, free throw attempts, steals, and turnovers) during home and away games against the Raptors in the playoffs. Two bar charts (field goal percentage, shooting percentage, free throw percentage) at home and away games against the Raptors during playoffs. We see the Cavaliers putting up high averages against the Raptors, especially in free throws and field goal/three-point percentage. Their scoring efficiency and defensive plays against the Raptors are areas Toronto can learn from. These insights are crucial for the Raptors' strategists. By studying the Cavs' approach in these winning matches, particularly their home game tactics against strong teams like Washington, Atlanta, and Chicago, and away game strategies against Miami, the Raptors can refine their game plans for the next season.

To sum up, our analysis provides a clear picture of where the Toronto Raptors and Cleveland Cavaliers stand. We've pinpointed strengths and opportunities that can guide off season training and strategy development. For the Raptors, focusing on elevating away game performance and playoff resilence is key. In closing, let's channel these insights into actionable strategies. For player development, addressing the playoff performances for stars like Lowry and DeRozan is vital. For team strategy, adopting and adapting successful plays from opponents will be our focus moving forward.
