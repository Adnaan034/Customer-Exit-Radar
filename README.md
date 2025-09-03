# Customer-Exit-Radar
Predicting customer Exit Radar using Logistic Regression, Decision Tree, and Random Forest.  End-to-end ML pipeline for customer churn prediction with classical models.  Customer Exit Radar prediction project with preprocessing, EDA, and model evaluation.  ML project: Customer Exit Radar prediction using Logistic Regression, Decision Tree, and Random Forest.

## 📊Dataset

Source: (Add dataset link, e.g. Telco Customer Churn or your dataset)
Target variable: Churn (1 = Yes, 0 = No)
Features: Demographics, usage patterns, billing info, etc.

## 🛠️Project Workflow

Data Cleaning & Preprocessing
Exploratory Data Analysis (EDA) with visualizations
Feature Engineering
Model Building: Logistic Regression, Decision Tree, Random Forest
Model Evaluation: Accuracy, Precision, Recall, F1-score, ROC-AUC
Comparison of Models
Predictions on new data

## 🔍 Exploratory Data Analysis (EDA)

In the EDA phase, I explored the Telco Customer Churn dataset to understand patterns and data quality:

Checked Missing Values → Verified null values in all columns (e.g., some in TotalCharges).

Outlier Detection → Used boxplots to check for unusual values in numerical columns (MonthlyCharges, Tenure).

Class Imbalance → Visualized the target variable (Churn) using countplots and found the data to be imbalanced.

Distribution Analysis → Plotted histograms and value counts to see how features like tenure and MonthlyCharges are distributed.

Correlation Analysis → Checked which features (e.g., Contract, Payment Method) are most strongly related to churn.

## ⚙️ Data Preprocessing

After EDA, I prepared the dataset for machine learning:

Dropped Irrelevant Columns

CustomerID → Unique identifier, no predictive power.

TotalCharges → Derived from Tenure × MonthlyCharges, hence redundant.

Handled Missing Values

Filled categorical nulls (e.g., gender) with mode.

Filled numerical nulls with median.

Encoding Categorical Variables

Applied Label Encoding to convert categorical features (e.g., gender, Partner, Contract) into numeric form.

Balanced Dataset

Used SMOTE (Synthetic Minority Oversampling Technique) to balance the target variable (Churn).

Feature Scaling

Applied StandardScaler to scale numerical features so that all features contribute equally to the model.

## 📊Visualization

<img width="931" height="560" alt="Image" src="https://github.com/user-attachments/assets/40e98272-1a45-40f7-b4bd-161b62db492d" />
<img width="932" height="657" alt="Image" src="https://github.com/user-attachments/assets/4409b048-ef1e-4a5d-be2f-b17fe3ca501d" />
<img width="934" height="795" alt="Image" src="https://github.com/user-attachments/assets/0f8ec3be-f262-4c04-ae26-cffb623e2894" />

## 📈Results (Final Output of Models)

**Logistic Regression → Accuracy: 78%, ROC-AUC: 0.79**

**Decision Tree → Accuracy: 79%, ROC-AUC: 0.78**

**Random Forest → Accuracy: 85%, ROC-AUC: 0.85 ✅ (Best Performer)**

## 📌 Key Insights

Random Forest gave the best balance between accuracy and recall.

Features like tenure, monthly charges, and contract type had the strongest influence on churn.

## 🧰 Tech Stack**

Python (pandas, numpy, scikit-learn, matplotlib, seaborn, joblib)

Jupyter Notebook

Git/GitHub

## 🙌 Acknowledgements

Dataset Source: IBM Telco Customer Churn Dataset (Kaggle)

Tools & Libraries: scikit-learn, pandas, numpy, matplotlib, seaborn, imbalanced-learn

Documentation Reference: scikit-learn documentation
