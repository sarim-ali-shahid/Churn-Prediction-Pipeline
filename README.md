# Sarim Ali Shahid (DHC-1724)

**NOTE:** Due to GitHub size restrictions, the trained model file (churn_pipeline.pkl, 65 MB) can't be uploaded. 

# 📌 Telco Customer Churn Prediction – ML Pipeline

## 🎯 Objective

The goal of this project is to build a **production-ready machine learning pipeline** using **Scikit-learn** to predict customer churn based on customer demographics, account information, and service usage data.

This work is part of my **AI/ML Engineering Advanced Internship (Task 2)**.

---

## 📂 Dataset

* **Source**: [Telco Customer Churn Dataset (Kaggle)](https://www.kaggle.com/blastchar/telco-customer-churn)
* **Rows**: \~7043 customers
* **Target Variable**:

  * `Churn` → **Yes (1)** = Customer left
  * `Churn` → **No (0)** = Customer stayed

**Features include**:

* Demographics (gender, senior citizen, partner, dependents)
* Services (phone, internet, streaming, etc.)
* Account details (contract type, tenure, billing, monthly charges, total charges)

---

## ⚙️ Methodology

1. **Data Preprocessing**

   * Missing values handled
   * Numerical features scaled with `StandardScaler`
   * Categorical features encoded with `OneHotEncoder`
   * Combined using `ColumnTransformer`

2. **Pipeline Construction**

   * Full pipeline built with Scikit-learn `Pipeline` API
   * Models:

     * Logistic Regression (baseline)
     * Random Forest Classifier (improved model)

3. **Hyperparameter Tuning**

   * Used `GridSearchCV` for Random Forest
   * Optimized for **F1-score**

4. **Evaluation**

   * Accuracy, Precision, Recall, F1-score
   * Confusion Matrix (visualized with heatmap)

5. **Export Model**

   * Final pipeline saved with `joblib` as `churn_pipeline.pkl`

---

## 📊 Results

* **Logistic Regression**

  * Accuracy: `XX%`
  * F1-score: `XX`

* **Random Forest (Best Model)**

  * Accuracy: `XX%`
  * F1-score: `XX`
  * Best Parameters: `{...}`

📌 *(Replace `XX` with your actual results after running the notebook)*

---

## 🚀 How to Run

1. Clone the repo:

   ```bash
   git clone https://github.com/your-username/Telco-Churn-Pipeline.git
   cd Telco-Churn-Pipeline
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Run the notebook:

   ```bash
   jupyter notebook Telco-Customer-Churn.ipynb
   ```

---

## 📦 Files in Repo

* `Telco-Customer-Churn.ipynb` → Jupyter Notebook with pipeline implementation
* `WA_Fn-UseC_-Telco-Customer-Churn.csv` → Dataset (or download separately)
* `churn_pipeline.pkl` → Saved trained pipeline
* `requirements.txt` → Project dependencies
* `README.md` → Documentation

---

## 🧑‍💻 Author

**Sarim Ali Shahid** – BS Artificial Intelligence Student | AI/ML Engineering Intern at DevelopersHub Corporation

