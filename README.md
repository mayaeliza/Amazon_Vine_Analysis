# Amazon_Vine_Analysis
## Overview of the analysis: 
  - Use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, use PySpark, Pandas, or SQL to determine if there is any bias toward favorable reviews from Vine members in the dataset.

## Resources
  - PySpark, SQL, AWS RDS

## Performing ETL on Amazon Reviews
#### Extract
  - Pick a dataset from the Amazon Review datasets and extract the dataset into a DataFrame
  <img width="1261" alt="extract" src="https://user-images.githubusercontent.com/72039212/115576648-55490480-a289-11eb-9144-8626da57f647.png">

#### Transform
  - Transform the DataFrame into four separate DataFrames that match the table schema in pgAdmin
  <img width="1262" alt="transform 2" src="https://user-images.githubusercontent.com/72039212/115577148-c7214e00-a289-11eb-8ff2-d6c1687ad511.png">
  <img width="1261" alt="trans2" src="https://user-images.githubusercontent.com/72039212/115577204-d4d6d380-a289-11eb-881c-c483b95a3cf3.png">
#### Load
  - Ex: Loading review_id_table into SQL
<img width="1171" alt="LOAD into sql" src="https://user-images.githubusercontent.com/72039212/115575711-73623500-a288-11eb-8a7d-0901af378a26.png">

## Results:
  #### How many total reviews were there?
  - Total Reviews
    - 4,850,360
  - Total Reviews from Helpful Votes
    - 61,948

  #### How many reviews were 5 stars? 
  - 5 Star Total Reviews
    - 3,040,120
  - 5 Star Total Reviews from Helpful Votes
    - 32,804

  
  #### What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
  - 5 Star Vine Reviews %
    - 0.6329679956329451 
    - 63.30% of Vine reviews were 5 stars.
    
  - 5 Star Vine Reviews from Helpful Votes %
    - 0.0053175617525936395
    - .53% of helpful Vine reviews were 5 stars.
    
  - 5 Star Non-Vine Reviews %
    - 0.5809048951172375
    - 58.10% of non-Vine reviews were 5 stars.
    
  - 5 Star Non-Vine Reviews from Helpful Votes %
    - 0.01770078628978882
    - 1.77% of helpfulnon-Vine reviews were 5 stars.

## Summary: 
  #### Is there any positivity bias for reviews in the Vine program. 
