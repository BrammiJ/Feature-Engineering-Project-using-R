# Feature-Engineering-Project-using-R
Performed Feature Engineering using R on London Airbnb Dataset

The project was submitted as a solution to one of my coursework challenges- 2023-24 CST4070 Applied Data Analytics - Tools, Practical Big Data Handling, Cloud Distribution

### Project Overview:
The following steps were undertaken as part of this project:

**1. Data Exploration:** Explored the dataset to gain insights into the features and their relationships. Are there any missing values, outliers, or data quality issues that need to be addressed? \
### Results of EDA:
![Top 20 listings in Airbnb Dataset](https://github.com/BrammiJ/Feature-Engineering-Project-using-R/blob/main/EDA%20plots/top%2020%20listings.png)
![Popular Airbnb Neighborhoods](https://github.com/BrammiJ/Feature-Engineering-Project-using-R/blob/main/EDA%20plots/popular%20airbnb%20neighborhood%20groups.png)
![Wordcloud](https://github.com/BrammiJ/Feature-Engineering-Project-using-R/blob/main/EDA%20plots/wordcloud.png)
![Popular Room Types](https://github.com/BrammiJ/Feature-Engineering-Project-using-R/blob/main/EDA%20plots/popular%20room%20types.png)
![Frequency of Number of Bedrooms](https://github.com/BrammiJ/Feature-Engineering-Project-using-R/blob/main/EDA%20plots/bedrooms%20frequency.png)
**2. Data Preprocessing:** Cleaned the dataset, handled missing values (if necessary), and encoded categorical variables (if necessary). \
### Null values before Data Cleaning:
![Null values before cleaning](https://github.com/BrammiJ/Feature-Engineering-Project-using-R/blob/main/EDA%20plots/null%20values-before.png)

### Null values after Data Cleaning:
![Null values after Data cleaning](https://github.com/BrammiJ/Feature-Engineering-Project-using-R/blob/main/EDA%20plots/null%20values-after.png)

**3. Feature Engineering:** Created a feature engineering model designed to predict rental revenue using the given features. Formulated features based on specific
hypotheses, incorporating initial speculative ideas.

### Formulated the following 4 features:
   #### FEATURE 1: amenities count 
   Hypothesis based on initial speculation: Higher the number of amenities, higher is the quarterly revenue of the listing
   #### FEATURE 2: host trust worthiness
   Hypothesis based on initial speculation: Higher the trustworthiness of the host, higher will be the quarterly revenue of the listing
   #### FEATURE 3: host acceptance rate category and host response rate category
   Hypothesis based on initial speculation: Faster the response rates and acceptance rates of the host, higher the chances of bookings. Hence higher quarterly revenue of the listing
   #### FEATURE 4: host experience
   Hypothesis based on initial speculation: Longer the experience of the host, higher will be the quarterly revenue of the listing
### Results of Feature Engineering:
1. quarterly_revenue feature was created by grouping the listings by quarter and taking the product of price and number of reviews for the listing. This feature will serve as target variable for further analysis on the data.
2. amenities_count feature was created from amenities column with the initial assumption that higher the number of amenities, higher will be the quarterly revenue
3. host_trustworthiness feature was created using the host_is_superhost and review_scores_rating features with the initial assumption that higher the trustworthiness of the host, higher will be the quarterly revenue
4. host_response_rate_category and host_acceptance_rate_category features were created from host_response_rate and host_acceptance_rate features with the initial assumption that higher the response and acceptance rates of the host, higher will be the chances of bookings. Hence, higher the quarterly revenue.
5. host_experience feature was created from the host_since feature with the initial assumption that longer the host has been in the platform, higher will be the quarterly revenue of the listing

### Dataset
Due to size constraints, I've added the link to the datasets used in this project
[Link to Dataset](https://insideairbnb.com/get-the-data/)
