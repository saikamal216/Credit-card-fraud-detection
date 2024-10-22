# Credit-card-fraud-detection
- This code performs credit card fraud detection using machine learning.

# Dataset 
- Drive =  https://drive.google.com/file/d/1YzUKVxvMFG4o1-E9kcG5NadntQVA_YeC/view?usp=sharing
- Dataset collected form dataworld.com = https://data.world/vlad/credit-card-fraud-detection

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

# 7. Feature Importance 
  - The code calculates and plots feature importance for three different machine learning models: Decision Tree, Random Forest, and Gradient Boosting.These models are used for credit card fraud detection, and the goal is to determine which financial transaction features are most indicative of fraudulent activity. 
  - The feature importance is derived from the models' internal mechanisms. For example, in a Decision Tree, a feature's importance is determined by how much it contributes to reducing the impurity of the tree's nodes. In Random Forest and Gradient Boosting, the feature importance is typically calculated based on the average reduction in impurity across all trees.
  - The plots show us which features are the most crucial for each model's prediction. For example, in the Gradient Boosting plot, you can see that some features (e.g., V14, V4, V10) have a significantly higher importance score than others. This suggests that these features are the strongest indicators of fraud, and the model relies on them the most to make predictions.


Overall, the code provides a comprehensive example of building a credit card fraud detection system, including data preparation, model training, evaluation, and a simple deployment example. It demonstrates how to deal with imbalanced datasets and how to compare the performance of different machine learning models for classification tasks. 
