# Arrest Prediction - Logistic Regression & Random Forest on LAPD Open Data

This project is part of my hands-on learning journey through the LinkedIn Learning + Wolfram Research Machine Learning Certificate. It demonstrates that **machine learning can be done using only a Chromebook and free tools** — no expensive hardware or cloud services needed.

## 🎯 Objective
Build a machine learning model that predicts whether a police stop will lead to an arrest, using open data from the LAPD. This project also aims to empower learners who are underrepresented in ML by showing that **you can get started with minimal resources**.

## 🚀 For Beginners: How This Project Helps You
If you're new to ML, this repo shows you:
- How to work in **JupyterLab** on a Chromebook or low-powered device
- How to use **open government data** for meaningful ML
- How to train interpretable models with **Logistic Regression** and **Random Forest**
- How to evaluate models with confusion matrices and fairness-aware metrics
- How to keep memory usage low using **sparse data** techniques

## 🧠 Models Used
- **Logistic Regression** – Fast, interpretable baseline
- **Random Forest Classifier** – Handles non-linearity, more robust to class imbalance
- *(XGBoost coming soon!)*

## 🧰 Tools & Technologies
- JupyterLab (web-based environment)
- Python 3 (runs on Pyodide or standard kernel)
- `pandas`, `scikit-learn`, `matplotlib`
- `scipy.sparse` for memory-efficient data handling

## 📊 Dataset
- **Source:** Los Angeles Police Department Open Data (filtered for relevant fields)
- **Features:** Crime description, area, victim sex, descent, time
- **Target:** Whether an arrest was made

## ⚙️ ML Workflow
### 1. Data Preprocessing
- Drop rows with missing sex/descent
- One-hot encode high-cardinality features
- Label encode smaller categories
- Convert data to sparse format to save RAM

### 2. Model Training
- Logistic Regression (with `class_weight='balanced'`)
- Random Forest Classifier (with `class_weight='balanced'`)

### 3. Model Evaluation
- Accuracy, Precision, Recall, F1-Score
- ROC-AUC Score
- Confusion Matrix Visualization (with `matplotlib`)

### 4. Inference Example (Coming Soon)
```python
# Example
Input: {'Vict Sex': 'M', 'Vict Descent': 'W', 'Crime': 'BATTERY', 'Area': 'Hollywood'}
Output: 0.71 (71% chance of arrest)
```

## 📁 Project Structure
```
notebooks/       - Jupyter notebooks for training and evaluation
data/            - Raw and cleaned datasets
README.md        - This file
```

## ✅ Next Steps
- [ ] Add XGBoost + early stopping
- [ ] Add SHAP or LIME for explainability
- [ ] Evaluate model fairness by race/gender
- [ ] Add binder link for 1-click launch (free cloud Jupyter)

## 💬 Final Note
This repo is meant to be a guide and proof that **you don’t need powerful hardware or paid services to start doing machine learning**. If you have access to a browser, you have access to ML.

Let's build together. ✊🏾💻🧠
