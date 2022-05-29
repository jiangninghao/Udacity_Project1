# Udacity_Project1
This is for the first project in Udacity Data Scientist nanodegree. Below is the table of contents for this file: 
1. Motivation of the project
2. Python library list
3. Dataset description
4. Functions applied 
5. Summary of the findings

## Motivation of the project 

As a seasoned analytical professional yet a novice data science practioner, this is the first hand-on exerice for me to practice my hands-on analytical skills via python coding. I chose the Seatle airbnb dataset provided by Udacity team to address the three questions as below: 
1. Which listing ID received the most reviews and which listing ID shows the highest average pricing?  
2. Which zipcode in the Seattle ara receives the highest average review score? 
3. If I want to predict the pricing, what are the most relevant features to use? 

## Python Library 
```python
- numpy
- pandas
- matplotlib
- seaborn

```

## Dataset description 

The first dataset named 'calendar' provides the time-series information of availability and pricing for each listing id over one year. 
The second dataset named 'reviews' provideds info on the counts of review per listing id. 
Combining these 2 datasets will allow us to figure out which listing id has the highest average pricing or the highest reviewer counts. 
The third dataset, which is the biggest dataset out of the three and the main dataset used for pricing predicting, is the listing. It provides key info, such as property details (e.g., # of bedroom, # of bathroom, # of beds, etc.), neighborhood detail, reviewer ratings by type, etc. 

## Fucntion used 
```python 

Two functions were used in this project

# The first function used is to covnert the price from string to float, which is used for avergae pricing calculation 

# The second funciton used is to treat the categorical columns
  
```

## Summary 
To answer the first two questions, data wrangling was applied to 1) convert targeted columns to the right format, 2) filled NAN files with 0s and 3) merge  'Calendar' and 'Review' dataset. It turned out that: 
  - Listing ID 208356 has the highest reviewer counts of 474 times and lsiting ID 3308979 has highest averag price of $1301.82. 
  - Area with zipcode of 98146 has the highest average rating of 98.0

To answer my 3rd question, I narrowed down the 'listing' data to a specific set (based on data content and business knowledge) and ran a correlation analysis to determine the most relevant features to pricing. Features including acocmandtes, bedrooms, beds, and bathrooms were identified and used in the pricing prediciton model. 
