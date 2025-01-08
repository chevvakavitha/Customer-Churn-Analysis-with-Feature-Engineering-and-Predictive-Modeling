# Customer Churn Analysis with Feature Engineering and Predictive Modeling
This project focuses on analyzing customer churn using predictive modeling techniques. The goal is to predict which customers are likely 
to churn (leave a service) based on historical data. Feature engineering plays a key role in improving model performance by creating new features from raw data.

---

## Table of Contents
- [Project Overview](#project-overview)
- [Data Description](#data-description)
- [Feature Engineering](#feature-engineering)
- [Predictive Modeling](#predictive-modeling)
- [Usage](#usage)
- [Installation](#installation)
- [Dependencies](#dependencies)
- [License](#license)

---

## Project Overview
Customer churn is a critical problem for businesses, as retaining existing customers is often more cost-effective than acquiring new ones.
This project uses **predictive modeling** techniques to identify potential churn risks and take proactive actions to retain valuable customers. 
Feature engineering techniques are applied to enhance the raw data and improve the model's predictive accuracy.

---

### The Key Steps in the Project:
1. Data preprocessing and feature engineering.
2. Model training and evaluation.
3. Predicting customer churn using different machine learning algorithms.
![image](https://github.com/user-attachments/assets/a5dc1686-a78c-40dd-9192-7d5b5efe2f3f)

---

## Data Description
The dataset used in this project contains historical data on customer behavior and attributes. Typical columns may include:
- `CustomerID`: Unique identifier for each customer.
- `Tenure`: The number of months the customer has been with the company.
- `MonthlyCharges`: The monthly cost of the service for the customer.
- `TotalCharges`: The total amount spent by the customer.
- `Churn`: Whether the customer has churned (1 = Yes, 0 = No).
- `Contract`: Type of contract the customer has (e.g., Month-to-month, One year, Two years).
- `PaymentMethod`: The customer's payment method (e.g., Electronic check, Mailed check, Bank transfer).
![image](https://github.com/user-attachments/assets/9dee55a9-c1b6-4ec7-9673-fc6a232e70ca)


Additional features may be created through **feature engineering**, such as:
- **Tenure Categories**: Categorizing customers based on their tenure (e.g., new, long-term).
- **Charge-to-Tenure Ratio**: Ratio of monthly charges to tenure, indicating if a customer is spending more over time.
![image](https://github.com/user-attachments/assets/0db37da1-99b6-49fa-a642-7c8d49edc243)

---

## Feature Engineering
Feature engineering is the process of using domain knowledge to create features that enhance the predictive power of machine learning models.
In this project, the following techniques were applied:
- **Handling Missing Data**: Imputing missing values using mean, median, or mode imputation techniques.
- **Categorical Encoding**: Converting categorical features into numerical formats (e.g., using one-hot encoding or label encoding).
- **Feature Transformation**: Normalizing or scaling features to bring all attributes to a similar range.
- **Creating Interaction Features**: Combining features (e.g., `Tenure * MonthlyCharges`) to capture relationships between them.
![image](https://github.com/user-attachments/assets/c2e60590-3e4b-42d5-aecd-398c824afe9b)

---

## Predictive Modeling
Several machine learning algorithms are applied to predict customer churn, including:
1. **Logistic Regression**: A baseline model to predict binary churn outcomes.
2. **Random Forest**: A decision-tree-based ensemble model for better accuracy.
3. **XGBoost**: A gradient boosting algorithm for high-performance predictions.
4. **Support Vector Machine (SVM)**: For classification in high-dimensional spaces.
![image](https://github.com/user-attachments/assets/9d11d132-e89f-4869-8834-ae15c3e368fe)

Model evaluation is done using performance metrics such as:
- **Accuracy**
- **Precision**
- **Recall**
- **F1-Score**
- **ROC-AUC**

---

## Usage
1. Clone this repository:
    ```bash
    git clone https://github.com/yourusername/customer-churn-analysis.git
    cd customer-churn-analysis
    ```

2. Load your dataset into the project.

3. Run the churn analysis script:
    ```bash
    python churn_analysis.py
    ```
4. The model's performance will be displayed, and the results will be saved to `churn_predictions.csv`.
5. You can also view model performance metrics such as accuracy and AUC in the output.

---

## Installation
1. Clone this repository:
    ```bash
    git clone https://github.com/yourusername/customer-churn-analysis.git
    ```

2. Navigate to the project directory:
    ```bash
    cd customer-churn-analysis
    ```

3. Install required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

---

## Dependencies
- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn
- xgboost
- imbalanced-learn
![image](https://github.com/user-attachments/assets/b1a89db5-1d8a-4c96-a28b-2758ba6a1fd5)

You can install the required dependencies by running:
```bash
pip install -r requirements.txt

---

## Conclusion
In this project, we successfully predicted customer churn using various machine learning models and feature engineering techniques.
By transforming raw data into meaningful features,we were able to enhance the model's performance and generate more accurate predictions.
The key steps included data preprocessing, handling missing values, encoding categorical features, and creating new interaction features.

### Key Insights:
- **Feature Engineering**: Feature creation, such as tenure categories and charge-to-tenure ratios, significantly improved the model's ability to predict churn.
- **Predictive Modeling**: Models like Logistic Regression, Random Forest, and XGBoost performed well in predicting churn, with XGBoost offering the best results.
- **Model Evaluation**: The evaluation metrics such as accuracy, precision, recall, and ROC-AUC provided deep insights
into model performance and helped in understanding the trade-offs between false positives and false negatives.

### Impact:
The ability to predict customer churn with high accuracy allows businesses to take proactive steps to retain valuable customers.
 By targeting customers at risk of leaving, companies can design personalized retention strategies, optimize marketing efforts, and improve customer satisfaction.

### Future Work:
- **Advanced Feature Engineering**: Explore additional features such as customer demographics or usage patterns to further improve prediction accuracy.
- **Time Series Analysis**: Incorporate time-dependent features or analyze churn trends over time to provide more dynamic insights.
- **Model Deployment**: Deploy the model into a production environment for real-time churn prediction.

Overall, this project serves as a foundation for businesses to better understand customer behavior and take actionable steps to improve retention rates and customer satisfaction.

