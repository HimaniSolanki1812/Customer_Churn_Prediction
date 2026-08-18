# Customer Churn Prediction

A Machine Learning project that predicts whether a telecom customer is likely to **churn (leave the company)** based on customer information and service usage.

This project was developed as part of my **Machine Learning internship at CodeC Technologies**.

---

## 📌 Project Overview

Customer churn is a major challenge for telecom companies. Identifying customers who are likely to leave can help businesses take preventive actions and improve customer retention.

In this project, a Machine Learning classification model is trained using the **Telco Customer Churn dataset** to predict whether a customer will:

* **Churn → Yes**
* **Churn → No**

This is a **Binary Classification** problem.

---

## 🎯 Objectives

* Understand and analyze customer churn data.
* Perform data cleaning and preprocessing.
* Explore relationships between customer characteristics and churn.
* Convert categorical data into numerical features.
* Train multiple Machine Learning classification models.
* Evaluate model performance using multiple metrics.
* Select the best-performing model.
* Save the trained model for future predictions.
* Create a Python prediction script for new customers.

---

## 🗂️ Dataset

The project uses the **Telco Customer Churn dataset**.

The dataset contains customer information such as:

* Gender
* Senior Citizen
* Partner
* Dependents
* Tenure
* Phone Service
* Multiple Lines
* Internet Service
* Online Security
* Online Backup
* Device Protection
* Tech Support
* Streaming TV
* Streaming Movies
* Contract
* Paperless Billing
* Payment Method
* Monthly Charges
* Total Charges

### Target Variable

`Churn`

Possible values:

* `Yes` → Customer left the company
* `No` → Customer stayed with the company

---

## 🛠️ Technologies Used

* **Python**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Seaborn**
* **Scikit-learn**
* **Jupyter Notebook**
* **Joblib**
* **Git & GitHub**

---

## 🔍 Project Workflow

The project follows these major steps:

```text
Dataset
   ↓
Data Loading
   ↓
Data Inspection
   ↓
Data Cleaning
   ↓
Exploratory Data Analysis
   ↓
Feature Engineering & Preprocessing
   ↓
Train-Test Split
   ↓
Model Training
   ↓
Model Evaluation
   ↓
Model Comparison
   ↓
Best Model Selection
   ↓
Model Saving
   ↓
Customer Churn Prediction
```

---

## 🧹 Data Preprocessing

The following preprocessing tasks were performed:

* Converted `TotalCharges` into numerical format.
* Handled missing values.
* Checked for duplicate customer records.
* Removed the `customerID` column because it is only an identifier.
* Separated features and target.
* Converted the target variable:

  * `No → 0`
  * `Yes → 1`
* Identified numerical and categorical features.
* Applied One-Hot Encoding to categorical features.
* Used a preprocessing pipeline with Scikit-learn.

---

## 📊 Exploratory Data Analysis

Several visualizations were created to understand customer behavior and churn patterns.

The analysis includes:

* Customer churn distribution
* Contract type vs churn
* Tenure vs churn
* Monthly charges vs churn
* Internet service vs churn

Some important patterns observed include:

* Month-to-month customers tend to have higher churn.
* Customers with shorter tenure tend to churn more frequently.
* Monthly charges can be associated with higher churn.
* Churn behavior varies across different service types.

These observations helped guide the Machine Learning process.

---

## 🤖 Machine Learning Models

The following classification algorithms were trained and compared:

### 1. Logistic Regression

Used as a strong baseline model for binary classification.

### 2. Decision Tree

Uses decision rules to classify customers.

### 3. Random Forest

Uses multiple decision trees to improve prediction performance.

### 4. Gradient Boosting

Builds models sequentially to improve classification performance.

---

## 📈 Model Evaluation

The models were evaluated using:

* **Accuracy**
* **Precision**
* **Recall**
* **F1-Score**
* **Confusion Matrix**

### Why multiple metrics?

Accuracy alone does not always provide enough information for a churn prediction problem.

For example, **Recall** is important because we want to identify as many customers who are actually going to churn as possible.

The **F1-score** provides a balance between Precision and Recall.

The final model was selected based on the overall evaluation results.

> **Note:** The exact performance values are available in the Jupyter Notebook and depend on the trained model and dataset split.

---

## 💾 Model Saving

The selected trained model is saved using Joblib.

Example:

```text
models/customer_churn_model.pkl
```

The saved model can later be loaded without retraining the model.

---

## 🔮 Making Predictions

The project includes a prediction script:

```text
src/predict.py
```

The script loads the saved Machine Learning model and can be used to generate churn predictions for new customer information.

Prediction output:

```text
Churn: Yes
```

or

```text
Churn: No
```

---

## 📁 Project Structure

```text
Customer_Churn_Prediction/
│
├── data/
│   └── customer_churn.csv
│
├── notebook/
│   └── customer_churn_prediction.ipynb
│
├── models/
│   └── customer_churn_model.pkl
│
├── images/
│
├── src/
│   └── predict.py
│
├── .gitignore
└── README.md
```

---

## ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/HimaniSolanki1812/Customer_Churn_Prediction.git
```

Navigate into the project:

```bash
cd Customer_Churn_Prediction
```

Install the required libraries:

```bash
pip install -r requirements.txt
```

---

## ▶️ Run the Project

### Jupyter Notebook

Open the project in VS Code and run:

```text
notebook/customer_churn_prediction.ipynb
```

Select the appropriate Python environment and execute the notebook cells in order.

### Prediction Script

The prediction script is located at:

```text
src/predict.py
```

Run it using:

```bash
python src/predict.py
```

---

## 📌 Future Improvements

Possible future improvements include:

* Hyperparameter tuning
* Cross-validation
* Handling class imbalance
* Feature importance analysis
* Model explainability
* Streamlit web application
* Cloud deployment
* Real-time customer churn prediction

---

## 🎓 Internship Project

This project was developed as part of my **Machine Learning internship at CodeC Technologies**.

It demonstrates practical understanding of:

* Data preprocessing
* Exploratory Data Analysis
* Binary Classification
* Machine Learning model training
* Model evaluation
* Model selection
* Model persistence
* GitHub project management

---

## 👩‍💻 Author

**Himani Solanki**

GitHub:
https://github.com/HimaniSolanki1812

---

## ⭐ Acknowledgment

Dataset: **Telco Customer Churn Dataset**
