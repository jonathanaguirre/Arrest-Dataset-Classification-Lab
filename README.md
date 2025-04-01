# Arrest Prediction - Classification with Logistic Regression and XGBoost

This project is part of my hands-on journey through the **LinkedIn Learning + Wolfram Research Machine Learning Certificate**. It explores supervised learning using real-world stop-and-search data to predict whether a police stop will lead to an arrest.

## 🎯 Objective  
Use classification algorithms to build a model that predicts arrest likelihood based on features like age, gender, time of day, and location.

## 🧠 Models Used  
- Logistic Regression  
- XGBoost (Python API)

## 🧰 Tools & Technologies  
- JupyterLab (Web-based)  
- Python 3.8 (Pyodide Kernel or standard kernel)  
- Pandas, Scikit-learn, XGBoost  
- Matplotlib or Plotly (for visualization)

## 📊 Dataset  
- Dataset: PLACERHOLDER  
- Features: PLACEHOLDER  
- Target: PLACEHOLDER

## ⚙️ ML Workflow  
1. **Data Preprocessing**  
   - KNN Imputation  
   - One-hot Encoding  
   - Outlier Removal  
   - Feature Correlation Analysis  

2. **Model Training**  
   - Logistic Regression using scikit-learn  
   - XGBoost Classifier (Python API)

3. **Model Evaluation**  
   - AUC (Area Under the Curve)  
   - Accuracy, Precision, Recall, F1-Score  
   - Confusion Matrix  
   - Output: Arrest Probability Score  

4. **Model Inference (Local)**  
   - Input new data into the trained model within the notebook  
   - Generate arrest probability scores directly

## 🔄 Example Inference  
> Input: Gender=Male, Age=25, Time=2PM, Ethnicity=White, Location=XYZ  
> Output: `0.71` (71% chance of arrest)

## 📁 Project Structure  
- `notebooks/` – Jupyter Notebooks for each stage (preprocessing, training, evaluation, inference)  
- `data/` – Raw and cleaned datasets  
- `models/` – Saved model files (`.pkl` or `.json`)  
- `outputs/` – Charts, confusion matrices, metrics reports

## ✅ Next Steps  
- Add SHAP or LIME for model explainability  
- Evaluate model fairness across demographics  
- Convert to U.S.-based dataset for further localization
