# Movies-ETL
## Overview
Management was pleased with the dataset and want to keep it updated on a daily basis.  They have requested to create an automated pipeline that takes in new data, transforms it and then loads it into a postgres database.  

### Results
Created a function to load all three datasources: wiki_movies, kaggle_metadata and ratings.
![ETLFunctionTest](https://github.com/john10roberts/Movies-ETL/blob/main/Data/ETL_function_test.ipynb)

Created and refactored the ETL function test code to extract and transform the wiki_movies data so that it could be merged with the kaggle_metadata.
![ETL_clean_wiki_movies](https://github.com/john10roberts/Movies-ETL/blob/main/Data/ETL_clean_wiki_movies.ipynb)

Created a process to extract and transform the kaggle_metadata and ratings data into dataframes.  The kaggle data will be merged with the wiki_movies to create a new data frame.  That data frame will be merged with the ratings data to create a final merged data frame containing all relevant information and ratings. 
![ETL_clean_kaggle_data](https://github.com/john10roberts/Movies-ETL/blob/main/Data/ETL_clean_kaggle_data.ipynb)

Refactored the code from the ETL_clean_kaggle_data to create a connection to a postgres database to automatially update the tables with new data. 
![ETL_create_database](https://github.com/john10roberts/Movies-ETL/blob/main/Data/ETL_create_database.ipynb)

Ran queries to verify that the data transfer was successful
![Movies Query](https://github.com/john10roberts/Movies-ETL/blob/main/Data/movies_query.ipynb)

![Ratings Query](https://github.com/john10roberts/Movies-ETL/blob/main/Data/ratings_query.ipynb)
