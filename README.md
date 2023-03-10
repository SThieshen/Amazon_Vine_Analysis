# Big Data

## Project Overview
As a data analyst for BigMarket, a startup that helps businesses optimize their marketing efforts, I've been hired to help a new client, Sellby, perform some pretty hefty analytics. Sellby is preparing to release a large catalog of products on a leading retail website. They want to know how the reviews of their products compare to the reviews of similar products sold by their competitors. They're also interested in enrolling in a program that gives free products to select reviewers, but they want to know if it's worth the cost. There are thousands of reviews and they're in words, not numbers. For this project, I'll translate them in order to analyze them. Sellby hired BigMarket because they believe in the power of big data.  

## Challenge Deliverables and Results

### Deliverable 1: Perform ETL on Amazon Product Reviews
Using knowledge of the cloud ETL process, an AWS RDS database with tables in pgAdmin was created. Then, using an Amazon Review dataset for wrist watches, I extracted the dataset into a DataFrame. I transformed the DataFrame into four separate DataFrames that match the table schema in pgAdmin. Finally, I uploaded the transformed data into the appropriate tables and ran SQL queries in pgAdmin to confirm that the data was uploaded.

### Deliverable 2: Determine Bias of Vine Reviews
Using my knowledge of PySpark, I performed analysis on the same Amazon Review dataset to see if there is any bias towards reviews that were written as part of the Vine program. For this analysis, I created multiple filtered DataFrames and performed calculations to determine if having a paid Vine review makes a difference in the percentage of 5-star reviews.

Based on the results of this analysis, I've answered the following questions:

### - **How many Vine (paid) reviews and non-Vine (unpaid) reviews were there?**

<img src="https://github.com/SThieshen/Amazon_Vine_Analysis/blob/main/development/images/total.png">

### - **How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?** 

<img src="https://github.com/SThieshen/Amazon_Vine_Analysis/blob/main/development/images/Del_2_total.png">

### - **What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?** 

<img src="https://github.com/SThieshen/Amazon_Vine_Analysis/blob/main/development/images/Del_2_5_star.png">

## Challenge Summary
In summary, the percentage of 5-star ratings for Vine reviews is 31.9% compared to 51.8% for non-Vine reviews, which clearly shows there is no bias for reviews in the Vine program. If there was a positive bias for Vine reviews, we would expect the opposite trend - that the percentage of 5-star ratings for Vine reviews to be higher than non-Vine reviews. To support this assertion further, I could perform statistical analysis to compare the distribution of reviews between the two groups, such as calculating the mean and mode for each subset.
