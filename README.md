## Overview

Telecom companies face significant challenges in retaining customers due to high churn rates. This project aims to **analyze telecom customer churn** using **exploratory data analysis (EDA)** and **machine learning models** to predict which customers are likely to churn.  

The analysis covers:  
- Understanding **customer demographics**, including age, gender, marital status, city, and zip code.  
- Examining **service usage patterns**, such as phone service, internet service, online security, streaming, and other subscriptions.  
- Investigating **contract types, payment methods, and offers** that may influence churn behavior.  
- Handling missing values, encoding categorical variables, and scaling numerical features for machine learning.  
- Building predictive models using **Random Forest, Gradient Boost, Extra Trees, AdaBoost, Decision Tree, KNN, XGBoost, and LightGBM**.  
- Evaluating models using **accuracy, cross-validation, confusion matrices, and classification reports**.  
- Identifying the **most important features** that drive churn decisions.  

The goal is to provide actionable insights and a robust predictive model to help telecom companies **reduce churn and improve customer retention**.


## Exploratory Data Analysis (EDA)

In this section, we explore the telecom customer dataset to uncover patterns and relationships that may influence churn. The EDA is divided into five parts for better clarity.

---

### 1. Overall Features

This section covers **general distributions** of categorical and numerical features, including:  
- Gender, marital status, city, zip code  
- Age distribution  
- Payment methods, contract types, and offers  
- Service usage (phone, internet, streaming, tech support, etc.)  

*Insert your overall insights here.*  

<img width="1920" height="1080" alt="Blue Modern Visual Data   Chart Presentation " src="https://github.com/user-attachments/assets/163402ef-5e8f-430b-9a27-c8d65ec2e50e" />
<img width="1920" height="1080" alt="4" src="https://github.com/user-attachments/assets/3d713681-72e7-475e-b464-cd79962fdb3c" />
<img width="1920" height="1080" alt="5" src="https://github.com/user-attachments/assets/0c6bf971-cfa6-420e-89f3-ce721b2d88d6" />
<img width="1990" height="1389" alt="download (7)" src="https://github.com/user-attachments/assets/2a95b313-8ca7-46c3-a820-43c98b520507" />


---

### 2. Effect by Gender

This section analyzes how **gender influences customer churn and service usage patterns**, including:  
- Distribution of services among male and female customers  
- Gender-wise differences in churn, contract types, and payment methods  

*Insert your gender-based insights here.*  

<img width="1589" height="2990" alt="download (1)" src="https://github.com/user-attachments/assets/8e2d3fca-d551-4256-81dd-42d72cb330b4" />


---

### 3. Effect by Marital Status

This section examines the impact of **marital status** on churn and service adoption:  
- Service subscriptions by marital status  
- Differences in contract types, payment methods, and churn behavior among married vs. unmarried customers  

*Insert your marital status insights here.*  

<img width="1589" height="2990" alt="download" src="https://github.com/user-attachments/assets/7a8aad67-3b13-4d4e-a1fd-d42f0edfd925" />


---

### 4. Effect by Top 20 Cities

This section focuses on **geographical patterns** by analyzing the top 20 cities with the highest customer counts:  
- Gender, service usage, payment methods, and contract types in each city  
- Offers adopted and churn distribution across cities  

*Insert your city-based insights here.*  

<img width="1785" height="3490" alt="download (4)" src="https://github.com/user-attachments/assets/e9ff6944-d041-4fc2-ac67-b8081232e652" />
<img width="1785" height="2090" alt="download (6)" src="https://github.com/user-attachments/assets/9a40d2d8-1d66-4e1c-a889-b5d36ae84d04" />



---

### 5. Effect by Age

This section explores how **age impacts churn and service adoption**, focusing on the top 20 ages by customer count:  
- Service usage patterns by age group  
- Contract types, payment methods, and churn behavior by age  

*Insert your age-based insights here.*  

<img width="1788" height="3490" alt="download (3)" src="https://github.com/user-attachments/assets/5d6bb479-a3cf-4d55-a7fe-b242992744dd" />



## Machine Learning Models

This section presents the predictive modeling results for **telecom churn**. Multiple machine learning algorithms were evaluated to identify the best-performing model.

### 1. Models Used

The following models were trained and evaluated:  

- **Random Forest Classifier**  
- **K-Nearest Neighbors (KNN)**  
- **Gradient Boosting Classifier**  
- **Extra Trees Classifier**  
- **Decision Tree Classifier**  
- **AdaBoost Classifier**  
- **XGBoost Classifier**  
- **LightGBM Classifier**

### 2. Evaluation Metrics

Models were evaluated using:  
- **Accuracy** on the test set  
- **10-fold cross-validation accuracy**  
- **Confusion matrix**  
- **Classification report** (Precision, Recall, F1-score)  
- **Feature importance** (for tree-based models)

### 3. Model Performance Summary

| Model             | Test Accuracy | Cross-Val Accuracy | Std Dev | Notes |
|------------------|---------------|-----------------|---------|-------|
| Random Forest     | 99.79%        | 99.79%          | 0.17%   | Excellent performance, very few misclassifications |
| KNN               | 72.18%        | 71.16%          | 1.59%   | Lower performance, struggled with minority class |
| Gradient Boost    | 100.00%       | 100.00%         | 0.00%   | Perfect accuracy on this dataset |
| Extra Trees       | 96.95%        | 97.60%          | 0.81%   | Slightly lower recall for minority class |
| Decision Tree     | 100.00%       | 100.00%         | 0.00%   | Perfect accuracy |
| AdaBoost          | 100.00%       | 100.00%         | 0.00%   | Perfect accuracy |
| XGBoost           | 100.00%       | 100.00%         | 0.00%   | Perfect accuracy |
| LightGBM          | 100.00%       | 100.00%         | 0.00%   | Perfect accuracy |

> **Note:** Test Accuracy and Cross-Validation Accuracy are nearly identical, indicating consistent model performance.

---

### 4. Confusion Matrices

The confusion matrix for each model is visualized below:  



- **Random Forest:**
 <img width="528" height="393" alt="rf" src="https://github.com/user-attachments/assets/d41e5c36-7b96-43c5-9ae6-b83b346faed9" />
- **KNN:**
 <img width="528" height="393" alt="knn" src="https://github.com/user-attachments/assets/f4cbc569-35e8-405c-9bee-49afc63c47b9" /> 
- **Gradient Boost:**
 <img width="528" height="393" alt="gb" src="https://github.com/user-attachments/assets/0bb587c9-925f-43cf-9135-e42668706260" />
- **Extra Trees:**
  <img width="528" height="393" alt="et" src="https://github.com/user-attachments/assets/fb1eb138-a2ab-462f-8fbb-f75c5555582f" />
- **Decision Tree:**
   <img width="528" height="393" alt="dt" src="https://github.com/user-attachments/assets/514f2566-af9d-46f4-a7e9-3e3c93f5eee6" />
- **AdaBoost:**
  <img width="528" height="393" alt="ab" src="https://github.com/user-attachments/assets/f9e48ae0-2fc3-428d-8fa4-4b93765ba20e" />
- **XGBoost:**
  <img width="528" height="393" alt="xgb" src="https://github.com/user-attachments/assets/16bb4180-eb1a-40bf-b0bb-38a58ef3a6a9" />
- **LightGBM:**
  <img width="528" height="393" alt="lbgb" src="https://github.com/user-attachments/assets/3972a940-00f3-4e9b-a388-ad61cf2eca1d" />








---

### 5. Feature Importance

For tree-based models (Random Forest, Gradient Boost, Extra Trees, AdaBoost, XGBoost, LightGBM), the **top 20 most important features** were identified to understand the key drivers of churn.  

*Insert bar plots of feature importance here for each tree-based model.*  

These insights help highlight which customer attributes and services most strongly influence churn behavior.

---

### 6. Key Takeaways

- **Gradient Boost, Decision Tree, AdaBoost, XGBoost, and LightGBM** achieved perfect accuracy on this dataset.  
- **Random Forest and Extra Trees** also performed extremely well, with minor misclassifications in minority classes.  
- **KNN** struggled to classify minority classes effectively, indicating that distance-based methods may be less suitable for this dataset.  
- Feature importance analysis provides actionable insights for **customer retention strategies**.

