# Zomato Restaurant Clustering and Sentimen Analysis

## Problem Statement

Zomato is an Indian restaurant aggregator and food delivery start-up founded by Deepinder Goyal and Pankaj Chaddah in 2008. Zomato provides information, menus and user-reviews of restaurants, and also has food delivery options from partner restaurants in select cities. 
India is quite famous for its diverse multi cuisine available in a large number of restaurants and hotel resorts, which is reminiscent of unity in diversity. Restaurant business in India is always evolving. More Indians are warming up to the idea of eating restaurant food whether by dining outside or getting food delivered. The growing number of restaurants in every state of India has been a motivation to inspect the data to get some insights, interesting facts and figures about the Indian food industry in each city. So, this project focuses on analysing the Zomato restaurant data for each city in India.
The Project focuses on Customers and Company, you have to analyze the sentiments of the reviews given by the customer in the data and made some useful conclusion in the form of Visualizations. Also, cluster the zomato restaurants into different segments. The data is vizualized as it becomes easy to analyse data at instant. The Analysis also solves some of the business cases that can directly help the customers finding the Best restaurant in their locality and for the company to grow up and work on the fields they are currently lagging in.
This could help in clustering the restaurants into segments. Also the data has valuable information around cuisine and costing which can be used in cost vs. benefit analysis.Data could be used for sentiment analysis. Also the metadata of reviewers can be used for identifying the critics in the industry.

### **Business Problem Analysis**

Indian cuisine consists of a variety of regional and traditional cuisines native to the Indian subcontinent. With every state, you can find something different to love. Besides traditional North Indian and South Indian food, the food culture is heavily inspired by and evolved around various civilizations. To say that Indians are food lovers would be an understatement. 
The restaurant business in India has been booming and people even like to celebrate small occasions of their lives with good food and great ambiance. 
Here comes Zomato, connecting people and restaurants.
Zomato is an Indian restaurant aggregator which provides information, menus, and user reviews of restaurants, and also has food delivery options. They basically take orders on the restaurant's behalf and get the food delivered at the convenience of your doorstep.

The problem statement here has two datasets for us to work on:
* Zomato Restaurant Names and Metadata
* Zomato Restaurant Reviews

To assure Zomato's success it is important for the company to analyze its datasets and make appropriate strategic decisions. The problem statement here asks us to cluster the restaurants to help customers find the best restaurants in their city and according to their taste and understand the fields they are lagging in. This will help Zomato in building a good recommendation system for their customers. Do a cost-benefit analysis using the cuisines and costs of the restaurants.
In order to understand fields that need to be worked upon, it is important to do sentiment analysis to get an idea about how people really feel about a particular restaurant. To identify the industry critics and  especially work on their reviews to build a reputation worth praising.


### **Notebook Breakdown:**
* Business Problem Analysis
* Data Collection
* Data Cleaning and Preprocessing
* Feature Engineering
* Exploratory Data Analysis
    - Best Restaurants in the City
    - The Most Popular Cuisines in Hyderabad
    - Restaurants and their Costs
    - Cost-Benefit Analysis
    - Hypotheses Generation on visualized data for Clustering
* Restaurant Clustering
    - K means Clustering on Cost and Ratings
    - Multi-Dimensional K means Restaurant Clustering 
        -  Principal Component Analysis
        -  Silhouette Score
        -  K means Clustering
        -  Cluster Exploration
* Sentiment Analysis 
    -  Exploratory Data Analysis
        -  Critics in the Industry
    -  Text Pre-Processing and Text Visualization
    - Modeling
* Conclusion


 ## Conclusion
- During our analysis we performed EDA on both numerical and categorical feature. We have dropped various unncessary columns and also added new columns which was very helpful for out clustering process. 

* After Analysis we have gathered some info which is given as following -> 

1. All top 10 Restaurants have higher rating than 4. Whereas AB's Absolute Barbecues has the highest rating of 4.88.**
2. The average rating of Restaurants falls mostly in range of 3 to 4 stars.
3. North Indian, Chinese and Continental foods are the most available cuisines in the Restaurants. Whereas, Indonesian, North-Eastern and Mexican are the least available cuisines in the Restaurants.
4. The top 3 costiest restaurants in Hyderabad are - 
    - Collage - Hyatt Hyderabad Gachibowli with cost of 2800 per person
    - Feast - Sheraton Hyderabad Hotel with cost of 2500 per person
    - Jonathan's Kitchen - Holiday Inn Express & Suites with cost of 1900 per   person.
5. The top 3 Cheapest restaurants in Hyderabad are -
    - Mohammedia Shawarma with cost of 150 per person
    - Amul with cost of 150 per person
    - Asian Meal Box with cost of 200 per person.
6. Most of the restaurants fall in the range of 500-1000 INR.



We have performed clustering over Cost and Avg Rating of the restuarants. And we have got Following clusters. - 
- Label 0 are those restaurants whose reviews wasn't present.  
- Label 1 are the restaurants whose rating is high and cost is low.
- Label 2 are fine dining restaurants with good ratings and average pricing.
- Label 3 restaurants are small food joints with whose rating is average but cost is very low.
- Label 4 are expensive restaurants that also had above-average ratings.

Sentiment Analysis were done on the Reviews and after model implementation we were getting accuracy for train data as 92% and for test data it is 89% using Logistic Regression. 
Hence we can deploy this model.  
