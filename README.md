# 🏦 Bank Customer Attrition Insights

This project analyzes customer data from a retail bank to identify the factors influencing customer attrition (i.e., customers leaving the bank). The goal is to build a classification model that predicts whether a customer is likely to exit, enabling proactive retention strategies.

---

## 📂 Data

The dataset used is:

- `Bank-Customer-Attrition-Insights-Data.csv`

It contains the following features:

- **Demographics**: `Age`, `Gender`, `Geography`  
- **Account Info**: `CreditScore`, `Balance`, `NumOfProducts`, `HasCrCard`, `IsActiveMember`  
- **Behavioral**: `Complain`, `Card Type`  
- **Target Variable**: `Exited` (1 if the customer left the bank, 0 otherwise)

---

## 🔍 Analysis Workflow

The project follows this structured workflow:

- Dataset loading and structure inspection  
- Missing values and duplicates check  
- Exploratory Data Analysis (EDA) using **Matplotlib** and **Seaborn**  
- Outlier clipping and data cleaning  
- Encoding of categorical features (`LabelEncoding` and `OneHotEncoding`)  
- SMOTE oversampling to address class imbalance  
- Feature selection using **ANOVA F-test**  
- Train/test split and standardization  
- Model training using:
  - **Random Forest Classifier**
  - **Logistic Regression**
- Evaluation using metrics like **accuracy**, **confusion matrix**, and **classification report**

---

## 📊 Key Insights

- No missing or duplicate values found  
- Strong correlations observed between features like `Age`, `Complain`, and the target `Exited`  
- Top predictive features: `Complain`, `Age`, `IsActiveMember`, `Gender`, `Geography`, and `NumOfProducts`  
- SMOTE effectively balanced the classes for better model learning  
- Outliers in features like `CreditScore` and `Age` were clipped to improve model stability

---

## 🤖 Model Performance

- **Random Forest Classifier**:
  - High accuracy and balanced performance across classes
  - Best-performing model in this project

- **Logistic Regression**:
  - Slightly lower performance, but strong interpretability
  - Suitable alternative for quick insights and simpler deployment

---

## 📁 Scripts & Outputs

- `Bank Customer Attrition Insights.ipynb`: Full pipeline from data preprocessing to model evaluation  
- Visual outputs include:
  - Distribution plots for numeric features
  - Count and pie plots for categorical features
  - Correlation heatmap
  - Confusion matrices and classification reports

---

## 🛠️ Libraries Used

- **Data Processing**: `pandas`, `numpy`  
- **Visualization**: `matplotlib`, `seaborn`  
- **Modeling**: `sklearn`, `imblearn` (SMOTE)  
- **Feature Selection**: `f_classif` from `sklearn.feature_selection`

---

## ✅ Usage

To run the project:

1. Clone this repository  
2. Place `Bank-Customer-Attrition-Insights-Data.csv` in the root directory  
3. Open and run the Jupyter notebook `Bank Customer Attrition Insights.ipynb`  
4. Review the EDA, feature analysis, and model performance

---

## 🚀 Future Improvements

- Experiment with additional classifiers (e.g., XGBoost, LightGBM)  
- Tune hyperparameters for better model performance  
- Explore time-based churn prediction if temporal data is available  
- Deploy the best model as an API or integrate into a customer dashboard

---

## 👤 Author

**Rohit Shivhare**  
[LinkedIn](https://www.linkedin.com/in/rohit-shivhare-a857a4233/)  
*MSc Data Science – Brunel University, London*
