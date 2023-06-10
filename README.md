# Data_mining_CRISP_I
Unveiling Airline Passenger Satisfaction with CRISP-DM Methodology

## Objective:
The aim of this project is to assist airlines companies in identifying crucial factors that significantly influence customer satisfaction. Given the pivotal role customer satisfaction plays in a company's success, it is imperative to thoroughly analyze and enhance the factors that closely correlate with customer contentment.

### Approach:
This project employs the CRISP-DM (Cross-Industry Standard Process for Data Mining) methodology to deliver a well-founded solution for the business challenge at hand. The project progresses through six distinct phases, namely Business Understanding, Data Understanding, Data Preparation, Data Modeling, Evaluation, and Deployment. Each phase contributes to a comprehensive understanding of the factors affecting passenger satisfaction and facilitates effective decision-making.

### Significance:
By employing the CRISP-DM methodology, this project empowers airlines companies to make data-driven decisions aimed at improving customer satisfaction. Identifying and addressing the key factors influencing passenger contentment can lead to enhanced growth and reputation within the industry. This project not only helps optimize the customer experience but also contributes to the long-term success and profitability of the airlines involved.

## About Dataset:
The dataset utilized in this project was obtained from Kaggle, encompassing data derived from an airlines' survey that gauged passenger satisfaction levels across a range of factors. The dataset comprises 25 columns, including demographic information such as Age and Gender, as well as details pertaining to travel class, Arrival and Departure delays, and various features influencing customer satisfaction, such as On-board service, Cleanliness, Seat comfort, and Baggage handling.

Of particular interest within the dataset is a column named 'satisfaction,' which serves as the measure of overall customer satisfaction. This column encompasses two distinct values: 'neutral or dissatisfied' and 'satisfied.' Serving as the label feature, this 'satisfaction' column consolidates the customer's overall experience based on their ratings of other features.

The dataset consists of 103,904 records for training purposes and 25,976 records for testing purposes, facilitating a robust analysis of passenger satisfaction.

### Content
**Gender:** Gender of the passengers (Female, Male)

**Customer Type:** The customer type (Loyal customer, disloyal customer)

**Age:** The actual age of the passengers

**Type of Travel:** Purpose of the flight of the passengers (Personal Travel, Business Travel)

**Class:** Travel class in the plane of the passengers (Business, Eco, Eco Plus)

**Flight distance:** The flight distance of this journey

**Inflight wifi service:** Satisfaction level of the inflight wifi service (0:Not Applicable;1-5)

**Departure/Arrival time convenient:** Satisfaction level of Departure/Arrival time convenient

**Ease of Online booking:** Satisfaction level of online booking

**Gate location:** Satisfaction level of Gate location

**Food and drink:** Satisfaction level of Food and drink

**Online boarding:** Satisfaction level of online boarding

**Seat comfort:** Satisfaction level of Seat comfort

**Inflight entertainment:** Satisfaction level of inflight entertainment

**On-board service:** Satisfaction level of On-board service

**Leg room service:** Satisfaction level of Leg room service

**Baggage handling:** Satisfaction level of baggage handling

**Check-in service:** Satisfaction level of Check-in service

**Inflight service:** Satisfaction level of inflight service

**Cleanliness:** Satisfaction level of Cleanliness

**Departure Delay in Minutes:** Minutes delayed when departure

**Arrival Delay in Minutes:** Minutes delayed when Arrival

**Satisfaction:** Airline satisfaction level(Satisfaction, neutral or dissatisfaction)

data source link: https://www.kaggle.com/datasets/teejmahal20/airline-passenger-satisfaction

## Data Cleaning and Exploratory Data Analysis for Improved Model Performance
Data cleaning and exploratory data analysis are critical steps in the machine learning process, enabling the derivation of accurate and reliable model outcomes. These steps involve identifying and addressing outliers, missing values, duplicates, and irrelevant data, as well as gaining a comprehensive understanding of the dataset through visual exploration. This project focuses on the cleaning and exploration of the dataset to enhance the subsequent model implementation.

### Data Cleaning:
One crucial aspect of data cleaning involves handling missing values and outliers. In this project, the 'Arrival Delay in Minutes' column was found to have 310 missing values. To address this issue, the missing values were imputed using the mean value calculated from the non-missing values within the same column. By filling in these missing values, the dataset becomes more complete and suitable for analysis.

### Exploratory Data Analysis:
Exploratory Data Analysis (EDA) plays a vital role in comprehending the dataset before implementing the model. It involves visually analyzing and summarizing the data to gain insights into its characteristics, distributions, and relationships among variables. Through EDA, patterns, trends, and potential correlations within the data can be uncovered, allowing for informed decision-making during subsequent modeling stages.

By performing thorough data cleaning and conducting comprehensive exploratory data analysis, this project lays the foundation for a robust and accurate model implementation, ensuring improved performance and more meaningful insights.


## Feature Correlation Analysis and Importance Evaluation for Enhanced Model Performance
Understanding the correlation among features and identifying the most relevant ones are essential steps in optimizing model performance. This project focuses on generating a correlation map to assess feature interdependencies and selecting the top ten features using the Chi-Square method. Additionally, the importance of features is determined through the application of Wrapper method and feature permutation importance technique. These techniques contribute to a more refined feature selection process, ultimately improving the overall effectiveness of the model.

### Correlation Analysis:
To gain insights into the relationship between features, a correlation map is generated. This map provides a visual representation of the correlation coefficients, enabling the identification of potential patterns or dependencies among the variables. By examining the correlation values, the project team gains a deeper understanding of how the features interact with each other, helping to identify potential redundancies or strong associations that can inform the subsequent feature selection process.

### Feature Selection:
The Chi-Square method is employed to select the top ten features from the dataset. This statistical test assesses the independence between categorical variables, allowing for the identification of features that are most likely to have a significant impact on the target variable. By focusing on these top-ranking features, the subsequent modeling process can prioritize the most influential factors, improving the model's predictive capabilities.

Additionally, the Wrapper method and feature permutation importance technique are utilized to evaluate the importance of features. The Wrapper method involves iteratively training and evaluating the model with different feature subsets, enabling the identification of the most optimal combination of features. The feature permutation importance technique assesses the impact of individual features by randomly permuting their values and measuring the resulting change in model performance. These techniques provide valuable insights into the relative importance of features, aiding in the selection of the most influential variables for the final model.

By conducting comprehensive feature correlation analysis and assessing feature importance through various techniques, this project aims to enhance model performance and ensure that the most relevant and impactful features are considered during the modeling process.


## Comparative Analysis of Eight Models for Optimal Performance
This project employs a comparative analysis approach to evaluate the performance of eight different models. By assessing various algorithms, we aim to identify the most efficient model for the given task. The models under consideration are Logistic Regression, Naive Bayes, KNN (K-Nearest Neighbors), Decision Tree, Neural Network, Random Forest, XGBoost, and AdaBoost. Each model brings unique characteristics and capabilities to the table, making this analysis crucial for selecting the most suitable approach.

### 1. Logistic Regression: 
This model is widely used for binary classification tasks, leveraging a linear regression framework to estimate the probability of an event occurring.

### 2. Naive Bayes: 
Based on Bayes' theorem, Naive Bayes is a probabilistic classifier known for its simplicity and speed. It assumes independence among features, making it particularly effective when dealing with text classification or spam filtering.

### 3. KNN (K-Nearest Neighbors): 
KNN is a non-parametric algorithm that classifies samples based on their proximity to other data points. It assigns labels by considering the majority class among the k nearest neighbors.

### 4. Decision Tree: 
Decision trees create a flowchart-like structure to make decisions based on feature values. This model is intuitive, easy to interpret, and suitable for both classification and regression tasks.

### 5. Neural Network: 
Inspired by the human brain, neural networks utilize interconnected layers of artificial neurons to process and learn from data. They excel in capturing complex relationships and are highly effective in various domains.

### 6. Random Forest: 
Random Forest combines multiple decision trees to form an ensemble model. It leverages the wisdom of crowds, improving predictive accuracy and handling high-dimensional datasets.

### 7. XGBoost: 
Extreme Gradient Boosting (XGBoost) is a powerful gradient boosting framework known for its speed and performance. It employs a combination of decision trees and gradient boosting techniques to achieve high accuracy.

### 8. AdaBoost: 
AdaBoost (Adaptive Boosting) is an ensemble method that iteratively adjusts the weights of misclassified samples, focusing on challenging instances to improve model performance.

By exploring these diverse models, this project aims to identify the most efficient and accurate approach for the specific task at hand, ultimately enabling better decision-making and improved outcomes.


## Optimal Model Selection: Random Forest Outperforms AdaBoost
After evaluating the performance of Random Forest and AdaBoost models, it is clear that both models achieved high ROC_AUC scores (~90%). However, Random Forest demonstrated superior efficiency, requiring less time for model training and prediction. Therefore, Random Forest is the recommended choice as the best-performing model for this project.
