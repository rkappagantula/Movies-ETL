# Movies-ETL

#### *ETL pipeline on movie data using Python and postgreSQL*

## Overview
This project consisted on a automated Extraction, Transformation and Load pipeline. This ETL extracted movie data from wikipedia, kaggle, and MovieLens to clean it, transform it, and merge it using Pandas. The product was a merged table with movies and ratings loaded to PostgreSQL. 

## Resources
- Data sources:
  - movies_metadata.csv
  - ratings.csv
  - wikipedia_movies.json

- Software:
  - Python
  - PostgreSQL
  - Pandas
  - SQLAlchemy
  - Regular Expressions 

## Results
- Datasets uploaded to PostgreSQL for other users to analyze movie data
- 
![movies_query](https://user-images.githubusercontent.com/96051648/162040505-900852d6-cba4-4f07-86db-ddd8384adc6e.png)

![ratings_query](https://user-images.githubusercontent.com/96051648/162040536-b663d0b2-df2a-458c-b014-bbbd48b65547.png)

## Summary
The pipeline was created under the following assumptions:
- Join the wikipedia, kaggle, and ratings movie data on the IMDB ID column.
- The wikipedia dataset didn't have a IMDB ID, ID is extracted from the url link given. 
- Each dataset was cleaned as there were duplicaes, null values incorrect data types etc.. 
- Wikipedia movie data was in json format. 
- Not every every movie had a rating for each rating level. 
- The ratings dataset had more than 26 million entries which generated a time constraint and a processing data challenge.



