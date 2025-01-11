# 💳 Credit Score Type Prediction 📊

## 📜 Project Overview

The goal of this project is to predict the credit score of customers based on their financial and transactional data. Accurate prediction of credit scores is essential for financial institutions to assess creditworthiness, manage risks, and make informed lending decisions.

## 🧑‍💻 Dataset Explanation

The dataset contains detailed information about customers, including demographic, income, credit, and payment behavior attributes. Below is a summary of the key features:

| **Column Name**             | **Description**                                               |
|-----------------------------|---------------------------------------------------------------|
| **ID**                       | Unique identifier for each transaction.                       |
| **Customer_ID**              | Unique identifier for each customer.                          |
| **Month**                    | Transaction month (as a numeric value).                       |
| **Name**                     | Full name of the customer.                                    |
| **Age**                      | Age of the customer (in years).                               |
| **SSN**                      | Social Security Number of the customer.                       |
| **Occupation**               | The customer's profession or job type.                        |
| **Annual_Income**            | The customer's total yearly income.                           |
| **Monthly_Inhand_Salary**    | Monthly take-home salary of the customer.                     |
| **Num_Bank_Accounts**        | Number of bank accounts the customer owns.                    |
| **Num_Credit_Card**          | Number of credit cards owned by the customer.                 |
| **Interest_Rate**            | Average interest rate on the customer's loans.                |
| **Num_of_Loan**              | Total number of loans taken by the customer.                  |
| **Type_of_Loan**             | Types of loans the customer has (e.g., Auto Loan, Personal Loan). |
| **Delay_from_due_date**      | Average delay (in days) for payments beyond the due date.     |
| **Num_of_Delayed_Payment**   | Number of payments delayed by the customer.                   |
| **Changed_Credit_Limit**     | Percentage change in the customer's credit limit.             |
| **Num_Credit_Inquiries**     | Number of credit inquiries made about the customer.           |
| **Credit_Mix**               | The diversity of credit types the customer uses (e.g., Good, Bad). |
| **Outstanding_Debt**         | Total outstanding debt of the customer.                       |
| **Credit_Utilization_Ratio** | Percentage of credit limit utilized by the customer.          |
| **Credit_History_Age**       | Age of the customer's credit history (in years).              |
| **Payment_of_Min_Amount**    | Indicates whether the customer pays the minimum amount due ("Yes" or "No"). |
| **Total_EMI_per_month**      | Total Equated Monthly Installments paid by the customer.      |
| **Amount_invested_monthly** | Monthly investment amount by the customer.                    |
| **Payment_Behaviour**        | Pattern of customer payments (e.g., High spent, Low spent).   |
| **Monthly_Balance**          | Average monthly balance after expenses.                       |
| **Credit_Score**             | Target variable indicating the customer's creditworthiness (Good, Bad, Standard). |

## 🔧 Key Techniques

- **Data Preprocessing**: Handling missing values, encoding categorical variables, and scaling numerical features.
- **Feature Engineering**: Extracting valuable features from the raw data.
- **Modeling**: Various classification models were applied, including Random Forest, K-Nearest Neighbors, Decision Trees, and Gradient Boosting.
- **Evaluation Metrics**: The models were evaluated using accuracy, precision, recall, and F1-score.

## 📈 Results and Observations

After applying several classification models, the following results were observed:

| **Model**                     | **Accuracy Score** |
|-------------------------------|--------------------|
| **Random Forest Classifier**   | **0.81575**        |
| **KNeighbors Classifier**      | **0.77585**        |
| **Decision Tree Classifier**   | **0.77115**        |
| **Gradient Boosting Classifier**| **0.70880**        |
| **Bernoulli NB**               | **0.62250**        |
| **Gaussian NB**                | **0.61720**        |
| **Logistic Regression**        | **0.54175**        |

- **Random Forest Classifier** performed the best with an accuracy of **81.57%**. Its classification report revealed:
  - **Good** credit scores: 78% precision and 78% recall.
  - **Poor** credit scores: 80% precision and 84% recall.
  - **Standard** credit scores: 84% precision and 82% recall.
  - Weighted average F1-score: **82%**.

- When a deep learning approach was used, accuracy dropped significantly to **53%**, which was lower than even simpler models like Logistic Regression.

Thus, traditional machine learning models like Random Forest outperformed deep learning methods for this dataset.

## 🚀 Hugging Face Space

You can try the interactive model for credit score prediction at the following link:
[Credit Score Type Prediction on Hugging Face](https://huggingface.co/spaces/Senasu/Credit_Score_Type_Prediction)

## 📥 Dataset

The dataset for this project can be accessed from the following link:
[Credit Score Classification Dataset](https://statso.io/credit-score-classification-case-study/)
