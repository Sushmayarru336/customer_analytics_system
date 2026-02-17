# Customer Churn Segmentation System: Churn Prediction & Behavioral Segmentation

## Project Summary

This project develops a complete machine learning workflow to understand customer behavior, predict churn risk, and segment customers into meaningful groups.

The objective is to transform raw customer data into actionable business insights that can support retention strategy and revenue protection.

---

##  Business Context

Customer churn is one of the biggest challenges for subscription-based businesses. 

Rather than reacting after customers leave, companies need predictive systems that:

- Identify customers likely to churn
- Understand behavioral patterns
- Group customers based on engagement and value
- Support proactive retention strategies

This project addresses those challenges using both supervised and unsupervised learning techniques.

---

##  Dataset Overview

The analysis uses the Telco Customer Churn dataset, which contains:

- Customer demographics
- Subscription services
- Contract information
- Billing details
- Tenure
- Churn status

---

##  Workflow & Methodology

### 1️. Data Preparation

- Removed non-informative identifiers (e.g., customerID)
- Converted `TotalCharges` into numeric format
- Handled missing values
- Encoded categorical variables
- Applied feature scaling using StandardScaler

---

### 2. Feature Engineering

To improve behavioral understanding, a new feature was created:

**Recency = Maximum Tenure − Individual Tenure**

This allows identification of relatively newer vs long-standing customers.

The churn variable was converted to binary format:
- Yes → 1
- No → 0

---

### 3️. Customer Segmentation (Unsupervised Learning)

KMeans clustering was applied to group customers into four distinct segments based on scaled behavioral attributes.

To improve interpretability, Principal Component Analysis (PCA) was used to reduce dimensionality for visualization.

---

##  Cluster Visualization

PCA-based 2D projection of customer segments:

![Cluster Visualization](images/cluster_visualization.png)

---

##  Tools & Technologies

- Python
- Pandas & NumPy
- Scikit-learn
- KMeans Clustering
- Principal Component Analysis (PCA)
- Matplotlib

---

##  Key Outcomes

- Identified distinct behavioral customer groups
- Highlighted potential high-risk churn segments
- Differentiated loyal, price-sensitive, and low-engagement customers
- Built a foundation for targeted retention campaigns

---

##  Potential Enhancements

- Deploy as a predictive API
- Integrate interactive dashboards (Streamlit / Power BI)
- Add automated retention recommendations using LLMs
- Perform hyperparameter optimization for clustering

---

##  What This Project Demonstrates

- End-to-end ML workflow
- Feature engineering strategy
- Supervised + unsupervised learning integration
- Business-driven data analysis
- Model visualization and interpretation

---

## Future Scope:
Integrating LLMs to auto-generate personalized retention recommendations based on churn probability and customer segment.

---

## 👤 Author

Sushma Yarru  
Python developer | Machine Learning Enthusiast | Data Science Learner  

Open to collaboration and feedback.
