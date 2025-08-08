# Bias and Fairness in Educational System AI

## 📌 Overview
This project analyzes bias in AI models used for educational predictions.
Two datasets were used:
- **Adult Census Income Dataset** – Predict income level.
- **Student Performance Dataset** – Predict student grade classification.

The objective is to evaluate fairness across gender, ethnicity, and parental education,
using fairness metrics and mitigation techniques.



## 🎯 Objectives
- Identify biased trends across demographic groups.
- Evaluate models using fairness metrics:
  - Demographic Parity Difference
  - Disparate Impact Ratio
  - Equalized Odds Difference
- Compare bias across datasets.
- Apply bias mitigation techniques without major loss in accuracy.



## 📂 Datasets
1. **Adult Census Income** – Demographic and occupational attributes.
2. **Student Performance** – Student demographics, parental background, academic factors.

## 🛠 Methodology

### 1. Data Preprocessing
- Handled missing values:
  - Mode imputation (categorical)
  - Mean/median imputation (numerical)
- Encoded categorical variables (Label Encoding, One-Hot Encoding).
- Standardized continuous features (z-score normalization).

### 2. Dataset Mapping & Analysis
- Mapped equivalent attributes (e.g., education levels, gender).
- Adopted a comparative analysis due to dataset structure differences.

### 3. Model Development
- Algorithm: Logistic Regression (for interpretability).
- Separate train-test split for each dataset.

### 4. Fairness Evaluation
- Tools: IBM AI Fairness 360 (AIF360), Fairlearn.
- Metrics:
  - Demographic Parity Difference
  - Disparate Impact Ratio
  - Equalized Odds Difference
- Visualized fairness gaps with group-wise charts.

### 5. Bias Mitigation
- Technique: Reweighing (AIF360) to adjust sample weights.
- Compared accuracy before and after mitigation.

---

## 💻 Tech Stack
- **Language:** Python
- **Libraries:** Pandas, NumPy, Scikit-learn, Seaborn, Matplotlib, Fairlearn, AIF360
- **Environment:** Jupyter Notebook



## 📊 Results Summary
- Gender bias: Minimal.
- Ethnicity & parental education bias: Significant in some metrics.
- Bias mitigation improved fairness without major accuracy loss.






##  How to Run

# Clone the repository
git clone <repo_link>

# Install dependencies
pip install pandas numpy scikit-learn seaborn matplotlib fairlearn aif360

# Run Jupyter Notebook
jupyter notebook bias_fairness.ipynb
