# Predictive Modeling for Customer Churn and Retention Analytics

### Project Overview

This project is an end to end data science initiative to proactively identify customers at high risk of churning. By analyzing a telco dataset, we build and evaluate several machine learning models to predict customer attrition. The final, optimized model can serve as a strategic tool for the business to inform targeted retention campaigns, ultimately aiming to enhance customer loyalty and protect revenue.

---

### Dataset

The dataset used for this project is the **Telco Customer Churn** dataset, which contains information about 7,043 customers and the services they subscribe to.

* **Source:** [Telco Customer Churn on Kaggle](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)

---

### Project Workflow 🚀

The project followed a structured, end to end machine learning workflow:

1.  **Exploratory Data Analysis (EDA):** Performed a deep dive into the data to understand distributions, identify correlations, and uncover key insights into the drivers of churn.
2.  **Data Preprocessing:** Cleaned the data and transformed it into a model ready format using one hot encoding for categorical features and standard scaling for numerical features.
3.  **Model Building:** Developed and trained four distinct classification models:
    * Logistic Regression (Baseline)
    * Decision Tree
    * Random Forest
    * XGBoost
4.  **Model Evaluation:** Compared the models based on key metrics like Accuracy, Precision, Recall, and F1-Score to select the best performer.
5.  **Hyperparameter Tuning:** Optimized the best performing model (XGBoost) using `GridSearchCV` to maximize its predictive power.
6.  **Final Evaluation:** Assessed the final, tuned model on the unseen test set to determine its real-world performance.

---

### Key Insights from EDA 📊

The analysis revealed several strong indicators of customer churn:

* **Contract Type:** Customers on **Month to Month contracts** churn at a significantly higher rate than those on yearly contracts.
* **Customer Tenure:** New customers with **low tenure** are at the highest risk of leaving.
* **Internet Service:** Customers with **Fiber Optic** internet have a higher churn rate compared to those with DSL.
* **Add-on Services:** Customers without key add ons like **Online Security** and **Tech Support** are more likely to churn.



---

### Final Model Performance 🏆

The final, tuned **XGBoost Classifier** was the best performing model for this task.

* **Accuracy:** **80%**
* **F1-Score (for the "Churn" class):** **58%**

The model demonstrates a strong ability to forecast customer attrition, providing a valuable tool to help the business strategically target retention efforts and reduce revenue loss.

---

### Technologies Used

* **Python:** The core programming language used for the analysis.
* **Libraries:** pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, XGBoost.
