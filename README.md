# ETL_Proj2

Team 8: Krystal Briggs and Rachel Song

We conducted an exploratory analysis of 120 years of the olympics. We want to look at whether the change of sports (inclusion/exclusion) decreased or increased the participation of female participants. 

Extract: Our original data source originated from Kaggle. We then formatted it through CSV and extracted the data using pgAgmin4/TablePlus.


Transform: We cleaned up the data by having to use Pandas to read in the CSV file because within the cells, the use of apostrophes made it read it as a special character and wouldn't initially import into our tables. We then transformed the data by selecting specific column names to print into a dataframe.


Load: Both 'athlete_events' and 'noc_regions' were chosen from our database 'olympics_db.'