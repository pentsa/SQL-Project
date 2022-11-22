# Sentiment analysis on Yelp
## Introduction
This projdct aims to investigate the buisnesses profile and user profile on Yelp for sentiment analysis. The project was completed using SQLite and the Yelp data from Coursea. The project first investigate the busineesses from food category in Toronto with high rating and low rating. By comparing the buisnesses, the project discovered that the ones with high rating usually have longer openning hour and more customer reviews, while no obvios trend in the neighborhood. The project then continued to look into the user profiles to compare the users with most fans and least fans in order to investigate the factors that contribute the fans number of the Yelp users. The popular users are the ones with more than 100 fans, while the unpopular users are the ones without any fans. The popular users tend to be on yelp for a longer period of time, and they have posted a lot of reviews that tend to receive more feedbacks as being ‘useful’, ‘funny’ and ‘cool’. When looking at the stars, there doesn’t seem to be a difference. In other words, the stars coming from the users won’t affect their popularity. This project allows Yelp to understand the user and business culture that allows them to be popular on Yelp.

## Features
- Database import
- Retriving for the buisness profiles from the food category in Toronto
  - Defining the businesses with high and low ratings 
  - Filtering for the location data for the target buisnesses
  - Filtering for the number of reviews for the target buisnesses
- Retriving the user accounts from Yelp with more than 100 fans or without any fans 
  - Comparing the similarities and differences between the popular and unpopular users
  - <img width="1293" alt="截圖 2022-11-21 下午2 19 38" src="https://user-images.githubusercontent.com/117743186/202979150-db0e6de2-1daa-4cda-a140-5bb9f48f0c87.png">

## Content 
- The entity relationship (ER) diagram for the Yelp database
  - <img width="655" alt="截圖 2022-11-21 下午2 33 46" src="https://user-images.githubusercontent.com/117743186/202981240-4d939fb9-2d91-49c9-baad-4b3d43213de0.png">
 
- Comparison of food buisnesses in Toronto with high and low ratings
  - Subqueries function was applied to find businessid from the food category in the category tabl
  - The case statement was applied to group the businesses by the star ranges to create a new column ‘rating’
  - The variables, such as neighborhood, postal_code, and review_count, were used as the comparisons between the two groups of buisnesses
  - The inner join function was applied to find the operation hours from the hours table using the matching business_id
- Comparison of user accounts with most and least fans to investigate the factors contributing to the popularity of the user accounts
  - Case statemnet was applied to definite the popularity of the users 
  - Users was grouped by the popularity to investigqte the anomalies between two groups
  - Number of reviews, types of feedbacks, and years of time on Yelp were retrieved to compare between the user groups
## Key findings
1. The businesses with 4-5 stars usually open in the afternoon with  shorter operation hours while the ones with 2-3 stars open in the morning.
2. The businesses with high rating have more reviews from the customers.
3. The popularity of the buisnees doesn't correlate with the location of the business
4. The popular users tend to be on yelp for a longer period of time, and they are active on Yelp with a lot of reviews that tend to receive more feedbacks  being ‘useful’, ‘funny’ and ‘cool’.  
5. When looking at the stars given by the users, there doesn’t seem to be a difference between the popular and unpopular users. In other words, the rating coming from the users doesn't affect their popularity. 

