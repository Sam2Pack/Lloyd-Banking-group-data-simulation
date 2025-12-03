<h1> Lloyd Banking group data job simulation</h1>
</br>
This was a data analysis and data science project.
<h2> About the data</h2>
</br>
The dataset comprises five CSV files containing customer data for a data science project focused on predicting churn status, the target variable indicating whether customers have left the service.​

File Overview
Churn_Status.csv: Lists CustomerID and ChurnStatus (e.g., values like 1 or 0), serving as the primary label for model training.​

Customer_Demographics.csv: Includes CustomerID, Age, Gender (M/F), MaritalStatus (Single/Married/Divorced/Widowed), and IncomeLevel (Low/Medium/High) for profiling customer segments.​

Transaction_History.csv: Records CustomerID, TransactionID, TransactionDate (2022), AmountSpent (numeric), and ProductCategory (Electronics/Clothing/Furniture/Groceries/Books) to analyze spending patterns.​

Online_Activity.csv: Tracks CustomerID, LastLoginDate (2023), LoginFrequency (1-49), and ServiceUsage (Mobile App/Website/Online Banking) for engagement metrics.​

Customer_Service.csv: Details CustomerID, InteractionID, InteractionDate (2022), InteractionType (Inquiry/Feedback/Complaint), and ResolutionStatus (Resolved/Unresolved) to capture support experiences.
</br>
<h2> About the solution</h2>
</br>
The solution consists of a proper exploratory data analysis of the data, understanding it, and drawing relations between different categorical features and how they affect the churn status. It also involoves preprocessing the data.
Then machine learning models have been made using svc, xgboost, random forest and a 4-layered neural network to see how well the prediction csn be done.
Class imbalance has also been taken care of using SMOTE. 
</br>
<h2>Results</h2>
</br>
The best model: XGboost classifier
performance metrics:
ROC_AUC score- 0.93
               precision    recall  f1-score   support

           0       0.97      0.97      0.97       846
           1       0.86      0.89      0.88       195

    accuracy                           0.95      1041
   macro avg       0.92      0.93      0.92      1041
weighted avg       0.95      0.95      0.95      1041
