## Predictive Modeling for Financial Health Assessment
**Objective**
The objective of this project was to develop a predictive model to assess and forecast the financial health of companies using various financial metrics. The goal was to predict the likelihood of financial instability or potential growth based on historical financial data.

**Dataset**
The dataset used for this project included various financial metrics of companies, such as:
Days Sales Outstanding (DSO)
Return on Assets (ROA)
Financial Expenses / Sales
Quick Ratio
Receivables Turnover
Debt to Assets Ratio
Inventory Turnover
Logarithm of Employees
Export Indicator
Import Indicator
Representative Indicator
Inconsistency Indicator (target variable)
Year

**Data Preprocessing**

**Handling Missing Values**
Missing values in the dataset were handled by filling them with the mean of the respective columns.

**Normalization**
The data was normalized using StandardScaler to ensure that all features have a mean of 0 and a standard deviation of 1, which is crucial for the performance of many machine learning algorithms.

**Data Splitting**
The dataset was split into training and testing sets using an 80-20 split.

**Exploratory Data Analysis (EDA)**

**Data Distribution**
The distribution of the target variable, Inconsistency Indicator, was visualized to understand the balance between the classes.
The distributions of key features were visualized to understand their spread and any potential skewness.

**Correlation Analysis**
A heatmap of the correlation matrix was created to visualize the relationships between different financial metrics. Key observations included:

A strong positive correlation between Quick Ratio and Return on Assets (ROA).
A strong negative correlation between Receivables Turnover and Days Sales Outstanding (DSO).

**Feature Engineering**

Principal Component Analysis (PCA)

PCA was applied to reduce the dimensionality of the dataset while retaining 95% of the variance.

**Model Building**

Multi-layer Perceptron (MLP) Model
An initial MLP model was built and trained on the training data.

**Model Evaluation**

The model's performance was evaluated using various metrics such as accuracy, precision, recall, F1-score, and ROC-AUC.

**Conclusion**

The model showed a high level of accuracy and other performance metrics, but the scenario analysis indicated that the Quick Ratio might not be a significant predictor of financial inconsistency. Further feature engineering and hyperparameter tuning could improve the model's sensitivity to key financial metrics. Additionally, exploring alternative models such as Gradient Boosting Machines (GBM) or XGBoost could provide better insights and predictive performance.
