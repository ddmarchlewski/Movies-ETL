# Movies-ETL
## Purpose
The purpose of this project was to use ETL to create an automated pipline, extract the data form multiple sources, use pandas to clean and transform the data automatically, and load the new data into PostgreSQL.

## Analysis
The analysis was split into four parts. 
- Write a function that reads the three data files and creates three seperate dataframes. 
- Extract, clean and transform the Wiki data and merge it with the Kaggle metadata.
- Extract, clean and transform the Kaggle metadata and MovieLens rating data, convert the transformed data into separate dataframes, merge the Kaggle metadata DataFrame with the Wikipedia movies dataframe to create the movies_df, and merge the MovieLens rating data DataFrame with the movies_df to create the movies_with_ratings_df.
- Add movies_df datadrame and movielens rating CSV data to a SQL database. 
 
### ETL_function_test
The data is first extracted in CSV and JSON formats. Then it is transformed into a Pandas data frame. 

### ETL_clean_wiki_movies
The clean_movie function was used to combine the data of other languages into one alt_titles column. The change_column_name function organizes the column names. 

### ETL_clean_kaggle_data
