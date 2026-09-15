# EasyVisa – Work Visa Approval Prediction

## 📌 Problem Statement

The increasing number of visa applications makes manual processing difficult. This project uses Machine Learning to predict whether a visa application will be Certified or Denied and identify the factors that significantly influence visa approval outcomes.

---

## ⚙️ Tech Stack

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- SMOTE
- AdaBoost
- Gradient Boosting
- Hyperparameter Tuning

---

## 🔍 Approach

- Data Cleaning & Preprocessing
- Exploratory Data Analysis (EDA)
- Feature analysis and engineering
- Handling class imbalance using SMOTE and undersampling
- Model building:
  - Decision Tree
  - Random Forest
  - AdaBoost
  - Gradient Boosting
- Hyperparameter tuning using RandomizedSearchCV
- Model evaluation using:
  - Accuracy
  - Precision
  - Recall
  - F1-score
  - ROC-AUC
  - Confusion Matrix
- Precision-Recall curve analysis

---

## 📊 Model Performance

The final model comparison focused on tuned ensemble models.

| Model | Accuracy | Precision | Recall | F1-score | ROC-AUC |
|---|---:|---:|---:|---:|---:|
| AdaBoost – Undersampled | 75.79% | 54.99% | 78.00% | **64.50%** | 84.50% |
| XGBoost – Original | 77.51% | 58.14% | 72.30% | 64.45% | 84.76% |

> **Note:** The project report identifies tuned AdaBoost as the best model at the selected classification threshold based on F1-score, while Gradient Boosting demonstrated a stronger precision-recall trade-off across thresholds.

---

## 💡 Key Insights

- **Education level** is one of the strongest predictors of visa certification.
- Applicants with **prior job experience** have a higher likelihood of certification.
- **Prevailing wage** and wage structure influence certification outcomes.
- Annual wage structures show stronger certification likelihood than other wage units.
- Geographic factors such as continent and region of employment have relatively limited predictive influence.
- The model emphasizes identifying likely certified applications while accepting a higher false-positive rate.

---

## 🎯 Business Recommendations

- Prioritize highly educated and experienced applicants during initial screening.
- Encourage competitive wage offerings aligned with prevailing wage standards.
- Support employers in structuring roles and compensation packages appropriately.
- Focus decision-making on applicant qualifications rather than geographic factors.
- Use the model for early identification and additional review of borderline cases.
- Collect richer information about applicant skills, certifications, and role-specific requirements.
- Adjust classification thresholds depending on whether the objective is higher recall or higher precision.

---

## 📁 Project Files

- `easy_visa_project.ipynb` → Complete Python and Machine Learning workflow
- `reports/Easy Visa project.pdf` → Detailed project report

---

## 🚀 Future Improvements

- Deploy the model as a web application
- Experiment with additional boosting algorithms such as XGBoost and LightGBM
- Develop a real-time prediction system
- Further improve model interpretability and feature analysis
