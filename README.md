# ETL_Proj2

Team 8: Krystal Briggs and Rachel Song

# Purpose:
We conducted an exploratory analysis of 120 years of the Olympics. We looked at whether the change of sports (inclusion/exclusion) has decreased or increased the participation of female participants, and what this could mean for future coverage of female athletes in sports. 

# Extract: 
Our original data source originated from Kaggle (https://www.kaggle.com/heesoo37/120-years-of-olympic-history-athletes-and-results). We then formatted it through CSV and extracted the data using pgAgmin4/TablePlus.

# Transform: 
We cleaned up the data by using Pandas to read in the CSV files. We then transformed the data by selecting specific column names to print into a dataframe.

# Create Database and Load Dataframes into Database: 
Within the cells of the CSV files, the use of apostrophes made SQL Server read it as a special character and wouldn't initially have us import the CSV files into our tables. Both 'athlete_events' and 'noc_regions' were chosen from our database 'olympics_db.'

ETL Anaysis can be found in:  olympic_ETL.ipynb.
Graphs and comparison analysis can be found in: Olympics_ETL_Analysis.ipynb.

# Specific questions we were looking to find answers to were: 

1) What year did we see the highest influx of female participants?
2) What country has the hightest rising female participation in the Olympic games?
3) What sports included the highest female participation ? 
4) What is the highest ranking medal female Olympic participants have earn compared to male participants? 
5) What season showed the highest female participation in the Olympics, winter or summer? 

Through our data analysis we discovered that:

 1)The rate of women participation in the Olymics began to take shape in 1900 at a small number of 33. In fact, the first Olympic Games to even accept female participants was in the 1900 Games in Paris. In more recent years, 2016 (the data had dates up to 2016), we found that the highest influx of women participation was at an astounding 6,223 for both the summer and winter Olympics! In contrast, mens' Olympics began to take shape a little earlier than womens', in 1890, with 380 male participants. Conversely, similarly to women, male participation rose in 2016 with 7,465 total male participastion for both summer and winter Olympics. 

2) The countries with the highest rising female participation in the Olymics has been Yugoslavia, with 378 females participants competing through most recent years. This could be do to the fact that Yugoslavia has been the destination for the Olympic teams in countries near Yugoslavia.  

3) The sports with the highest total number of female participation is for Alpine Skiing in the winter Olympics and Athletics (track and field) for the summer Olympics.

4) The highest rank of medals won for women participants in the Olympics is Bronze, whereas for men it's been Gold. 

5) There was a a commonality found between male and female Olympic participants. Both sexes predominately participate in the summer Olympics rather than Winter. A major reason for this could be because the summer Olympics are more popular than the winter, and have more countries competing in the summer over winter. Winter is only popular for participants where winter sports are valued and practiced. 

## Results:
Through our results we have determined that even though the inclusion of female athletes in the Olympics has increased female participation, female atheletes still lack in representation in terms of high medal ranking (The highest medal ranking female athletes have is bronze, whereas men have gold), and masculine sports (wrestling), compared to male athletes.  

## Future Research: 

Given more time we would have conducted a comparison analysis to further look at medal rankings between female and male Olympic athletes to determine why more male athletes score gold over female participants, who as a majority score bronze. In order to determine this, we would have looked at attributes such as "Sport," specifically more masculine sports that female athletes participant in. There could be a possiblity that since fewer women participate in more masculine Olympic activities such as wrestling;there are fewer opportunities for women to score gold. There's also a possbiltiy that due to a lack of female sport coverage during the Olympics compared to men, there is less emphasis on female sports, especially masculine sports; therefore, these reasons could be contributing to fewer female athletes joining Olympic teams. However more research would be needed to determine these questions. 
