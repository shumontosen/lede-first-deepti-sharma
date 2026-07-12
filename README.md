# How good is India's Deepti Sharma, the bowler

## Description
Indian all-rounder Deepti Sharma become the [leading wicket-ticker in women's international cricket](https://www.cricbuzz.com/cricket-news/139375/stats-how-deepti-sharma-rose-to-the-top-of-the-wickets-charts-in-womens-international-cricket-cricbuzzcom) after she sent Australia's Beth Mooney back to the pavilion during the team's last group game at the ICC Women's T20 World Cup on June 28, 2026. After that game, she had 356 wickets across all the formats of international cricket, Test matches, One-Day Internationals(ODIs) and T20 Internationals(T20Is), to her credit. By doing so, she went past former Indian fast bowler Jhulan Goswami's tally of 355 international wickets.

Using data I wanted to see how good she has been compared to other bowlers in all the three formats of international cricket. The analysis for all players was as of the final of the ICC Women's T20 World Cup played on July 5, 2026. 

## Findings
Out of Deepti's 356 international wickets, 168 were in T20 Internationals, the shortest and the most popular format of the game (which ends is played over three-four hours). This is understandable since 52% of her career has been T20Is. She has 166 scalps in ODIs (played over a day) and the rest 22 in Tests, the longest five-day format of the sport.

The data show that she is among the world's all-time best bowlers in the format. Not so much in the shorter formats.

She has played for India in only 10 Test innings (a Test match has typically two innings of batting and bowling each but it isn't necessary that every bowler will bowl in both the innings). And since there are much fewer Test matches played in the women's game, it is likely that such records won't be talked about so often.

## Collecting the data
All data used for the story is from ESPN Cricinfo's Statsguru. I scraped the data for the 200 bowlers with the highest wickets in each of the three formats using Pandas. Statsguru already had all of the data in a structured way so Pandas was sufficient in sourcing the data.

## Analysing the data
Most of the data analysis was done using Pandas and some of it was done using Google Sheets. 

After scraping, the data was collated into one dataframe because I first wanted to establish that Deepti was indeed international cricket's highest wicket-taker. I then added a column for each bowler classifying the format their stats were from. After that, I added another column classifying the countries the players represented into  Full Members or Associate Members. 

The International Cricket Council classifies countries playing cricket into two buckets, Full and Associate Members. Full Members are those countries wherein cricket is an established sport while Associate Members are those countries where the game is still developing. For purposes of this story, I have take only full members of the sport. 

I then added the wickets picked by all bowlers across formats. Based on that I was able to show that she indeed became the highest wicket-taker across all formats.

To see where Deepti stood compared to others, I picked two indicators each for each format to highlight a bowler's performance. They were:
1. Test matches: Strike rate (the number of balls per wicket) and Bowling Average (the number of runs conceded per wicket)
2. ODIs: Strike Rate (the number of balls per wicket) and Economy Rate (the number of runs conceded per over)
3. T20Is: Strike Rate (the number of balls per wicket) and Economy Rate (the number of runs conceded per over)

Now among bowlers in cricket, the lesser the value of the indicators mentioned above, the better the performance of the bowler. For example, a low strike rate indicates a bowler has bowled fewer balls per wicket. 

I then plotted the above indicators for every bowler in three scatter plots, one for each format. Here I used another cut-off. Since I wanted to show Deepti among bowlers who have bowled consistently, I plotted those bowlers who had picked at least:

1. 20 wickets in Tests
2. 70 wickets in ODIs
3. 50 wickets in T20Is

I then divided the scatters into quadrants. The quadrants were made based on the average of the two indicators used for each scatter. Players who were in the bottom-left quadrant were those who are elite. 

## Learnings

The biggest learnings from this project were knowing how to publish a project on the web and setting up and using ai2html for graphics. I always wanted to understand how to the script works to make Illustrator graphics responsive and how to integrate ai2html in a webpage. I also gained some confidence in how to use pandas for data analysis, data cleaning and data organising. I also learnt how to work with HTML and CSS to customise various aspects of my webpage.

## What more I would have liked to do

I wished I had more time to implement scrolly with my scatter plots to highlight more players