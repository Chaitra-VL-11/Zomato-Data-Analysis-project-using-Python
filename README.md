# 📌 Project Title: Zomato Customer and Restaurant Data Analysis

### ✅ Business Problem:
Zomato, one of the largest food delivery platforms in India, experiences a massive number of transactions each month. Understanding customer preferences and restaurant performance is crucial to improving customer experience, optimizing partner relationships, and driving strategic decisions.

Zomato wants insights into:
* Customer behavior across restaurant types
* Rating trends and user feedback
* Ordering preferences (online vs. offline)
* Spending patterns by customer segment (e.g., couples)

### 🎯 Project Objective:
To perform Exploratory Data Analysis (EDA) and derive actionable insights from customer and restaurant data, including:

* Understanding which type of restaurants are most popular
* Identifying rating trends
* Analyzing spending behavor
* Comparing online vs. offline order ratings
* Identifying opportunities for promotions and offers

### 🛠️ Tech Stack & Tools:
Language: Python
Libraries: pandas, matplotlib, seaborn, numpy
Environment: Jupyter Notebook / VS Code
Techniques:
Data Cleaning & Preprocessing
Exploratory Data Analysis (EDA)
Feature Engineering
Data Visualization
Type Conversion (rate column from string to float)

### 🔍 Data Preprocessing Example:
The rate column was originally in the format "4.1/5". To extract the numeric value:

def handleRate(value):

    value = str(value).split('/')
    value = value[0]
    return float(value)
    
dataframe['rate'] = dataframe['rate'].apply(handleRate)

### ❓ Key Business Questions & Insights:
* What type of restaurant do the majority of customers order from?
  
✅ Insight: Majority of orders are placed from Dining restaurants, showing high dine-in interest.

* How many votes has each type of restaurant received from customers?
  
✅ Insight: Dining restaurants received the most votes, indicating strong customer engagement and satisfaction.

* What are the ratings that the majority of restaurants have received?
  
✅ Insight: Most restaurants received ratings between 3.5 and 4.0, which indicates generally favorable customer experiences.

* What is the average spending per order among couples?
  
✅ Insight: Couples prefer restaurants with an average spending of approximately ₹300 per order.

* Which mode (online or offline) has received the highest ratings?
  
✅ Insight: Online orders received higher ratings compared to offline, suggesting better user satisfaction in digital experiences.

* Which type of restaurant received more offline orders?
  
✅ Insight:
Dining restaurants receive more offline orders, implying preference for on-premise experiences.
Cafes mostly receive online orders, opening opportunities for targeted digital promotions.

### 📈 Business Impact & Recommendations:
* Personalized Offers: Target dining restaurants with offline promotions, and cafes with online incentives.
* Improve Offline Experience: Since offline ratings are lower, focus on improving  in-restaurant service
* Customer Retention: Engage couples with combo offers or loyalty programs near the ₹300 price point.



