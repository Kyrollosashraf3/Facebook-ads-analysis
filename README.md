# Facebook Ads Analysis – Predictive Modeling

This project analyzes Facebook advertising campaign data to understand how pre-campaign factors impact performance outcomes.  
The goal is to predict whether a campaign will succeed or fail **before launch**, using only features like interest, budget, and age group.

## Dataset
- Source: Facebook Ads dataset (Kaggle)
- Includes demographic information (age, gender, interest) and campaign spending.
- Derived metrics:
  - CTR = clicks / impressions
  - CPC = spent / clicks
  - Conversion Rate = conversions / clicks

## Objective
- Analyze how features such as **age, gender, interest, and spent budget** influence campaign performance.  
- Build predictive models to classify campaign success/failure.  

## Data Wrangling
- Calculated new columns: CTR, CPC, Conversion Rate.
- Selected features available before campaign launch.
- Removed potential data leakage (post-campaign metrics).

## Models
- **Random Forest Classifier** – baseline model.  
- **Logistic Regression** – interpretable alternative.  
- Preprocessing with `ColumnTransformer` (OneHotEncoder + StandardScaler).  

## Evaluation
- Compared models using Accuracy, MSE, and R² metrics.  
- Random Forest achieved strong performance; Logistic Regression provided insights into feature importance.  

## Results
- Pre-campaign factors like **ad budget (Spent)** and **user interest** are significant predictors of success.  
- Logistic Regression allowed better interpretability of how each factor affects campaign success.  

## How to Run
1. Clone this repository.
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
