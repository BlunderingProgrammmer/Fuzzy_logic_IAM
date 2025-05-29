# Fuzzy Access Risk Prediction for Employee Attrition Data

## 📌 Overview

This project uses fuzzy logic and machine learning to simulate and predict employee access risk based on historical HR data. Risk is defined in terms of an employee's job level and income, helping HR departments assess the probability of insider threats or data access violations.

## 📊 Dataset

- **Source**: [IBM HR Analytics Employee Attrition Dataset](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset)
- **Size**: 1470 employee records
- **Features**: JobLevel, MonthlyIncome, JobSatisfaction, EnvironmentSatisfaction, etc.

## 🧪 Approach

1. **Simulate Access Risk**:
   - Custom rule: High Job Level + High Income → High Risk.
2. **Preprocessing**:
   - One-hot encoding, feature selection.
3. **Fuzzy Logic System**:
   - Membership functions for satisfaction levels, distance from home, etc.
4. **Random Forest Classifier**:
   - Trained on preprocessed data to predict risk.
5. **Model Explainability**:
   - SHAP used to explain predictions.
6. **Gradio Interface**:
   - Input employee data to get live risk classification.

## 📈 Results

- Random Forest shows robust classification performance.
- SHAP explains which features most contribute to high/low risk.
- Fuzzy logic enhances interpretability of decisions.

## 📦 Setup

```bash
pip install -r requirements.txt
```

Then run the notebook or launch the Gradio app for interactive use.

## 🧑‍💻 Author

- Built as part of an AI & Security exploration project.

## 📝 License

MIT License. See [LICENSE](LICENSE).
