# Credit-card-fraud-detection
- This code performs credit card fraud detection using machine learning.

# 1. Data Loading & Pre-processing:
  -It loads the credit card transaction dataset (CC.csv).
  - It explores the data using `data.head()` and `data.info()`.
  -  It removes unnecessary columns like 'Unnamed: 0'.

# 2. Data Visualization:
  - It visualizes the distribution of fraudulent (Class=1) and non-fraudulent (Class=0) transactions using a countplot.
  - It shows the distribution of transaction amounts using a histogram (`sns.displot`).
