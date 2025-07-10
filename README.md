# 🏋️‍♂️ Gym Customer Churn Prediction & Segmentation 
## 🔍 Overview
This project addresses customer churn prediction and segmentation for Model Fitness, a chain of gyms aiming to improve client retention through data-driven insights.

## 🎯 Objective
- Predict the likelihood of customer churn next month  
- Segment gym clients into meaningful clusters to understand different user profiles  
- Identify key factors influencing churn  
- Provide actionable recommendations to reduce churn and improve customer engagement  

## 📊 Dataset
The dataset includes user demographics, contract details, visit frequencies, and additional charges, covering two consecutive months. Key features include:

| Feature                   | Description                                                                                      |
|---------------------------|--------------------------------------------------------------------------------------------------|
| `Churn`                   | Whether the client churned in the current month (target variable)                                |
| `gender`                  | Gender of the client                                                                             |
| `Near_Location`           | Whether the client lives or works near the gym                                                  |
| `Partner`                 | Whether the client works at a partner company (eligible for discounts)                           |
| `Promo_friends`           | Whether the client signed up using a referral promo code                                        |
| `Phone`                   | Whether the client provided a phone number                                                      |
| `Age`                     | Age of the client                                                                               |
| `Lifetime`                | Number of months since the client first joined the gym                                          |
| `Contract_period`         | Contract length (1, 3, 6, or 12 months)                                                        |
| `Month_to_end_contract`   | Months left until contract expiration                                                          |
| `Group_visits`            | Participation in group sessions (yes/no)                                                       |
| `Avg_class_frequency_total`   | Average weekly visit frequency over lifetime                                                  |
| `Avg_class_frequency_current_month` | Average weekly visit frequency in the current month                                       |
| `Avg_additional_charges_total`   | Total money spent on additional services (cafeteria, products, massages, etc.)               |

## 🛠️ Methodology

1. **Exploratory Data Analysis (EDA):**  
   - Investigate missing values and feature distributions  
   - Compare averages and behavior patterns between churned vs. retained clients  
   - Visualize feature correlations and distributions  

2. **Churn Prediction Models:**  
   - Split data into training and validation sets  
   - Build and compare two classifiers: Logistic Regression and Random Forest  
   - Evaluate models using accuracy, precision, and recall metrics to select the best performer  

3. **Customer Segmentation:**  
   - Standardize data and perform hierarchical clustering to estimate optimal cluster count  
   - Apply K-means clustering (k=5) to group clients by behavioral and demographic similarities  
   - Analyze cluster characteristics and churn rates to identify high-risk and loyal groups  

4. **Conclusions & Recommendations:**  
   - Identify user profiles with higher churn risk such as low visit frequency and short contract length  
   - Suggest targeted retention strategies focusing on high-risk clusters with personalized offers  
   - Recommend encouraging group visits and leveraging partner company programs to improve loyalty  
   - Emphasize continuous monitoring of usage trends to proactively identify customers at risk  

---

## 🧰 Tools & Libraries
The project utilized the following Python libraries and tools for data analysis, modeling, and visualization:

- **pandas, numpy:** Data manipulation and numerical operations  
- **seaborn, matplotlib:** Data visualization and plotting  
- **scikit-learn:** Machine learning models and preprocessing  
  - Logistic Regression, Random Forest (classification)  
  - Train/test data splitting  
  - Model evaluation metrics (accuracy, precision, recall, F1-score, ROC AUC)  
  - K-means clustering and data scaling  
- **scipy:** Hierarchical clustering and dendrogram visualization  
