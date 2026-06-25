# Heart Disease Prediction

## Project Overview

This project predicts the likelihood of heart disease using machine learning techniques on a healthcare dataset. It includes data preprocessing, exploratory data analysis (EDA), model building, evaluation, and Power BI-based result visualization.

The project compares multiple machine learning models and identifies the better-performing model for heart disease prediction.

---

## Dataset Information

The dataset used in this project is **`heart.csv`**, which contains **303 patient records** and **14 attributes** related to heart health.

### Features in the dataset

* `age` – Age of the patient
* `sex` – Gender of the patient
* `cp` – Chest pain type
* `trestbps` – Resting blood pressure
* `chol` – Serum cholesterol
* `fbs` – Fasting blood sugar
* `restecg` – Resting electrocardiographic results
* `thalach` – Maximum heart rate achieved
* `exang` – Exercise induced angina
* `oldpeak` – ST depression induced by exercise
* `slope` – Slope of peak exercise ST segment
* `ca` – Number of major vessels colored by fluoroscopy
* `thal` – Thalassemia
* `target` – Heart disease presence

  * `0` = No Heart Disease
  * `1` = Heart Disease

---

## Project Workflow

### 1. Data Loading and Inspection

* Loaded the dataset using **Pandas**
* Displayed sample rows
* Checked dataset shape, data types, and missing values

### 2. Exploratory Data Analysis (EDA)

Performed analysis to understand the distribution and relationships in the dataset:

* Summary statistics using `describe()`
* Heart disease class distribution plot
* Age distribution comparison for patients with and without heart disease
* Correlation heatmap of all features

### 3. Data Preparation

* Defined input features (`X`) and target variable (`y`)
* Split the dataset into **training and testing sets**

  * **80% training**
  * **20% testing**

### 4. Model Building

Two machine learning models were trained and evaluated:

#### Logistic Regression

* Used as the primary classification model
* **Accuracy achieved: 88.52%**

#### Decision Tree Classifier

* Used for model comparison
* **Accuracy achieved: 75.41%**

### 5. Model Evaluation

* Compared model performance using **accuracy score**
* Generated a **confusion matrix** for Logistic Regression to evaluate predictions

### 6. Power BI Result Preparation

A final file named **`heart_disease_final_results.csv`** was generated for Power BI dashboard/report creation.

This file contains:

* original test feature values
* actual health status
* predicted health status

The labels were converted into readable categories:

* **Healthy**
* **Heart Disease**

---

## Technologies Used

* **Python**
* **Jupyter Notebook**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Seaborn**
* **Scikit-learn**
* **Power BI**

---

## Files in the Project

* **`Heart_disease_Analysis.ipynb`** – Jupyter notebook containing full analysis, preprocessing, model training, and evaluation
* **`heart.csv`** – Dataset used for heart disease prediction
* **`heart_disease_final_results.csv`** – Final prediction results prepared for Power BI
* **`heart disease prediction.pbix`** – Power BI dashboard/report file
* **`.gitignore`** – Ignores unnecessary files such as Jupyter checkpoints and Python cache files

---

## Model Performance Summary

| Model                    | Accuracy   |
| ------------------------ | ---------- |
| Logistic Regression      | **88.52%** |
| Decision Tree Classifier | **75.41%** |

### Best Performing Model

**Logistic Regression** performed better than Decision Tree in this project and was selected as the stronger model for heart disease prediction.

---

## Output of the Project

The project provides:

* heart disease prediction using machine learning
* comparison of classification models
* visual understanding of feature relationships
* final prediction results for dashboard creation in Power BI

---

## Future Improvements

* Apply feature scaling and hyperparameter tuning
* Try additional models such as Random Forest, SVM, and XGBoost
* Deploy the model using Flask / FastAPI / Streamlit
* Add an interactive web interface for prediction
* Expand the Power BI dashboard with more healthcare insights

---

## Conclusion

This project demonstrates how machine learning can be applied in healthcare to predict heart disease risk using patient data. By comparing models, the project shows that **Logistic Regression achieved better performance** on this dataset and can be used as an effective baseline model for heart disease prediction.
