# Telecom Customer Churn Analysis 📉

Exploratory Data Analysis (EDA) on telecom customer data to identify the key factors driving customer churn and help the business improve retention.

## 📊 About the Dataset

The dataset (`Customer_Churn.csv`) contains **7,043 customer records** across **21 columns**, including:

- `customerID`, `gender`, `SeniorCitizen`, `Partner`, `Dependents` — customer demographics
- `tenure` — number of months the customer has stayed with the company
- `PhoneService`, `MultipleLines`, `InternetService`, `OnlineSecurity`, `OnlineBackup`, `DeviceProtection`, `TechSupport`, `StreamingTV`, `StreamingMovies` — subscribed services
- `Contract`, `PaperlessBilling`, `PaymentMethod` — account/billing details
- `MonthlyCharges`, `TotalCharges` — billing amounts
- `Churn` — whether the customer left (target variable)

## 🛠️ Tools & Libraries

- Python
- Pandas & NumPy — data cleaning and manipulation
- Matplotlib & Seaborn — data visualization
- Jupyter Notebook

## 🧹 Data Cleaning

- Replaced blank values in `TotalCharges` with `0` (corresponding to customers with 0 tenure) and converted the column to `float`
- Checked for and confirmed no duplicate `customerID` entries
- Converted `SeniorCitizen` from binary (0/1) to readable Yes/No labels
- Verified no missing values remained after cleaning

## 🔍 Exploratory Data Analysis

The analysis explores churn patterns across:

- **Overall churn rate** — proportion of customers who churned vs. stayed
- **Gender** — churn distribution by gender
- **Senior Citizen status** — churn rate comparison
- **Tenure** — how length of relationship affects churn
- **Contract type** — churn by month-to-month vs. yearly contracts
- **Subscribed services** — impact of services like OnlineSecurity, TechSupport, StreamingTV, etc.
- **Payment method** — churn rate by payment type

## 📈 Key Insights

- **26.54%** of customers have churned overall
- Customers who are **Senior Citizens** churn at a noticeably higher rate than non-seniors
- Customers with **short tenure (1–2 months)** are far more likely to churn; long-tenured customers tend to stay
- Customers on **month-to-month contracts** churn significantly more than those on 1- or 2-year contracts
- Customers **without** services like OnlineSecurity, TechSupport, and OnlineBackup churn more often than those who have them
- Customers paying via **electronic check** show the highest churn rate among all payment methods

## ✅ Conclusion

> Churn is highest among customers with short tenure, month-to-month contracts, no add-on services (like OnlineSecurity/TechSupport), and electronic check as their payment method — senior citizens are also disproportionately affected. These segments should be prioritized for retention efforts such as contract incentives, bundled service offers, and proactive support outreach.

## 📁 Repository Structure
