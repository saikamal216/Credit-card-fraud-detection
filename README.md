# Credit-card-fraud-detection
- This code performs credit card fraud detection using machine learning.

# 1. Data Loading & Pre-processing:
  - It loads the credit card transaction dataset (CC.csv).
  - It explores the data using data.head() and data.info().
  - It removes unnecessary columns like 'Unnamed: 0'.

# 2. Data Visualization:
  - It visualizes the distribution of fraudulent (Class=1) and non-fraudulent (Class=0) transactions using a countplot.
  - It shows the distribution of transaction amounts using a histogram (sns.displot).

# 3. Feature Engineering:
  -  Addresses class imbalance by downsampling the majority class (non-fraudulent transactions).
  -  Combines the downsampled majority class with the minority class (fraudulent transactions) to create a balanced dataset.
  -  Splits the dataset into training and testing sets.


# 4. Model Training and Evaluation:
  - Trains three different machine learning models: Decision Tree, Random Forest, and Gradient Boosting.
  - Fits each model on the training data.
  - Makes predictions on the test data.
  - Evaluates the performance of each model using accuracy, confusion matrix, and classification report.

# 5. Model Comparison:
  -  Creates a bar chart to compare the accuracies of the three models.


# 6. Deployment Example:
  - Selects a few random rows from the dataset.
  - Uses the trained Random Forest model to predict fraud for these rows.
  - Compares the predicted values with the actual values to demonstrate the model's ability to detect fraud in real-time scenarios.


Overall, the code provides a comprehensive example of building a credit card fraud detection system, including data preparation, model training, evaluation, and a simple deployment example. It demonstrates how to deal with imbalanced datasets and how to compare the performance of different machine learning models for classification tasks. 
