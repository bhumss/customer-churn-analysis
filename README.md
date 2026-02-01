# Customer Churn Analysis & Prediction

In a subscription-based businesses model, customers leaving (churn) is a silent revenue killer.
This project explores why customers churn, who is most at risk, and how we can predict churn early using data and machine learning.

The goal is to turn insights into information that a business can actually use .

# Dataset

Dataset: Telco Customer Churn Dataset (Kaggle)

Records: 7,043 customers

Features: 21 columns

Target: Churn (Yes / No)

The dataset includes customer services used, contract details, and billing information —  to understand both customer behavior and business impact.

# Data Cleaning & Preparation

Dropped customerID (just an identifier, no predictive value)

Converted TotalCharges to numeric and handled missing values using median imputation

Encoded categorical variables with the help of encoders using :

Label Encoding for Yes/No columns

These steps ensured the data was clean, consistent, and model-ready.

# Exploratory Data Analysis (EDA)

Some patterns were identified from the data :

Month-to-month customers churn the most

New customers (low tenure) are far more likely to leave

Customers with higher monthly charges show higher churn

Lack of tech support or online security strongly correlates with churn

Visualizations using Matplotlib and Seaborn helped validate these trends and made them easier to explain to non-technical stakeholders.

# Feature Engineering

To improve model performance, a few smart features were added:

Average Monthly Spend → better reflects spending behavior

Groups → new, mid-term, and loyal customers

Feature Scaling → applied to numerical variables for better model stability

These transformations helped the models understand customer behavior more clearly.

# Models Used
## Logistic Regression

Used as a baseline

Easy to interpret

Helpful for understanding which features influence churn

## Random Forest Classifier

Captures non-linear patterns

Handles feature interactions well

Delivered stronger overall performance

# Evaluation Strategy

Instead of relying only on accuracy, the models were evaluated using:

Precision

Recall

F1-score

Confusion Matrix

Recall was the most important metric, because missing a customer who is about to churn is far more costly than reaching out to a loyal one.

Best Performing Model: Random Forest

# Business Takeaways

Here’s what I’d recommend:

Focus retention efforts on new and month-to-month customers

Encourage long-term contracts with targeted offers

Bundle services like Tech Support + Online Security

Keep eye on customers with high monthly bills

These actions can significantly reduce churn with minimal additional cost.

# Tools & Technologies

Python

Pandas & NumPy

Matplotlib & Seaborn

Scikit-learn

Jupyter Notebook
