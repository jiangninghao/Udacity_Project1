# Udacity_Project1
This is for the first project in Udacity Data Scientist nanodegree. Below is the table of contents for this file: 
1. Motivation of the project
2. Python library used
3. Data source
4. File description
5. Functions applied 
6. Summary of the results

## Motivation of the project 

As a seasoned analytical professional yet a novice data science practitioner, this is the first hands-on exerice for me to practice my hands-on analytical skills via Python coding. I chose the Seatle airbnb dataset provided by Udacity team to address the three questions below: 
1. Which listing ID received the most reviews and which listing ID shows the highest average pricing?  
2. Which zip code in the Seattle area receives the highest average review score? 
3. If I want to predict the pricing, what are the most relevant features to use? 

## Python Library used
- numpy
- pandas
- matplotlib
- seaborn

## Data Source
Data obtained from Seattle Airbnb Open data that is available on Kaggle (https://www.kaggle.com/datasets/airbnb/seattle)

## File description 
Seatle_Airbnb.zip contains 3 csv files: 
- calendar.csv:  provides the time-series information of availability and pricing for each listing id over one year. 
- reviews.csv: provides info on the counts of review per listing id. 
- listing.csv: the biggest dataset out of the three and the main dataset used for pricing predicting, is the listing. It provides key info, such as property details (e.g., # of bedrooms, # of bathrooms, # of beds, etc.), neighborhood details, reviewer ratings by type, etc. 

## Function used 
Two functions were used in this project.
The first function used is to convert the price from string to float, which is used for average pricing calculation 
The second function used is to treat the categorical columns

## Summary of the results
To answer the first two questions, data wrangling was applied to 
1) Convert targeted columns to the right format
2) filled NAN files with 0s 
3) merge  the 'Calendar' and 'Review' datasets. 

It turned out that: 
  - Listing ID 208356 has the highest reviewer counts of 474 times and listing ID 3308979 has the highest average price of $1301.82. 
  - Area with zipcode of 98146 has the highest average rating of 98.0

To answer my 3rd question, I narrowed down the 'listing' data to a specific set (based on data content and business knowledge) and ran a correlation analysis to determine the most relevant features to pricing. Features including commandoes, bedrooms, beds, and bathrooms were identified and used in the pricing prediction model. 

A more detailed summary is posted in my Medium blog (https://medium.com/@jiangninghao/lessons-learned-from-my-first-data-science-project-f5b4db773c38)

## Acknowledgements
This dataset is part of Airbnb inside. 
