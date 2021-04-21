# Amazon_Vine_Analysis
## Overview of the analysis: 

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
  #### How many Vine reviews and non-Vine reviews were there?
  #### How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
  #### What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

## Summary: 
  #### Is there any positivity bias for reviews in the Vine program. 
