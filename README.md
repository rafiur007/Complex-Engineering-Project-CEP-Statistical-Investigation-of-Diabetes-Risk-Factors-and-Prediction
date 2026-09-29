# 🩺 Pima Indians Diabetes Dataset: Statistical Analysis & Risk Factor Prediction


[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/rafiur007/Complex-Engineering-Project-CEP-Statistical-Investigation-of-Diabetes-Risk-Factors/blob/main/STAT_PR_CEP.ipynb)


An evidence-based statistical analysis and exploratory data science project executed in Python and Google Colab. This project applies statistical methods, probability theory, hypothesis testing, linear regression, and data visualization to analyze the **Pima Indians Diabetes Dataset** ($n = 768$, $p = 9$) and identify key clinical risk factors for diabetes.

---

## 📌 Table of Contents
- [Project Overview](#-project-overview)
- [Dataset Structure](#-dataset-structure)
- [Statistical & Methodological Framework](#-statistical--methodological-framework)
- [Key Findings & Analytical Results](#-key-findings--analytical-results)
- [Repository Structure](#-repository-structure)
- [How to Run in Google Colab](#-how-to-run-in-google-colab)
- [Tech Stack & Libraries](#-tech-stack--libraries)

---

## 📌 Project Overview

The objective of this study is to perform a rigorous exploratory and inferential analysis on female patients of Pima Indian heritage to investigate the physiological, demographic, and genetic factors associated with diabetes mellitus.

### Core Analytical Objectives:
1. **Dataset Inspection & Cleaning:** Evaluate dataset dimensions ($768$ rows, $9$ columns) and handle zero-value physiological anomalies in metrics like Glucose, BMI, Blood Pressure, and Insulin.
2. **Probability & Risk Analysis:** Compute empirical prior probabilities and conditional risk probabilities ($P(\text{Diabetes} \mid \text{Predictor})$).
3. **Distribution & CLT Verification:** Analyze distributional skewness and apply the Central Limit Theorem (CLT) to validate parametric testing.
4. **Inferential Hypothesis Testing:** Conduct Welch’s two-sample $t$-tests and $Z$-tests to evaluate mean parameter differences between diabetic ($\text{Outcome} = 1$) and non-diabetic ($\text{Outcome} = 0$) cohorts[cite: 8].
5. **Correlation & Regression Modeling:** Measure Pearson correlation coefficients ($r$)[cite: 5, 7] and build a Simple Linear Regression model to quantify age-dependent glucose trends[cite: 6].
6. **Risk Factor Ranking:** Synthesize statistical evidence to rank diabetes predictors by clinical impact[cite: 7, 8].

---

## 📊 Dataset Structure

The dataset comprises **768 observations** and **9 variables**:

| Variable Name | Data Type | Measurement Unit / Clinical Meaning |
| :--- | :---: | :--- |
| `Pregnancies` | `int64` | Number of times pregnant |
| `Glucose` | `int64` | Fasting plasma glucose concentration ($2$-hour oral glucose tolerance test, $\text{mg/dL}$) |
| `BloodPressure` | `int64` | Diastolic blood pressure ($\text{mm Hg}$) |
| `SkinThickness` | `int64` | Triceps skinfold thickness ($\text{mm}$) |
| `Insulin` | `int64` | 2-Hour serum insulin ($\mu\text{U/mL}$) |
| `BMI` | `float64` | Body Mass Index ($\text{kg/m}^2$) |
| `DiabetesPedigreeFunction` | `float64` | Diabetes hereditary pedigree score |
| `Age` | `int64` | Age in years |
| `Outcome` | `int64` | Binary diagnostic outcome ($0 = \text{Non-Diabetic}, 1 = \text{Diabetic}$) |

---

## 🔬 Statistical & Methodological Framework

The repository covers a 9-part analytical pipeline:

1. **Descriptive Statistics:** Summary statistics (mean, median, standard deviation, IQR, skewness) across all continuous metrics.
2. **Probability Theory:** Prior probability $P(D) \approx 0.349$ ($34.9\%$) and conditional risk evaluation[cite: 8].
3. **Distribution Analysis:** Density estimation using Kernel Density Plots (KDE) and boxplots to detect outliers and non-normal skewness[cite: 7, 8].
4. **Central Limit Theorem (CLT):** Sampling distributions of sample means converge to normality due to large subgroup sample sizes ($n_0 = 500, n_1 = 268$)[cite: 8].
5. **$95\%$ Confidence Intervals:** Calculation of non-overlapping parametric $95\%$ CIs for population parameters[cite: 8].
6. **Hypothesis Testing:** Independent Welch’s $t$-tests ($\alpha = 0.05$) to test $H_0: \mu_{\text{diabetic}} = \mu_{\text{non-diabetic}}$[cite: 8].
7. **Pearson Correlation Analysis:** Construction of feature correlation matrices and annotated heatmaps[cite: 5, 7].
8. **Simple Linear Regression:** Modeling $\text{Glucose} = \beta_0 + \beta_1 \times \text{Age}$ with slope significance testing ($p < 0.001$) and $R^2$ evaluation[cite: 6].
9. **Visual Diagnostics:** Comprehensive $2 \times 2$ Master Dashboard uniting probability, hypothesis testing, regression, and risk ranking[cite: 8].

---

## 📈 Key Findings & Analytical Results

* **Plasma Glucose is the Dominant Risk Factor ($r \approx +0.47, p < 0.0001$):**[cite: 7, 8]
  Diabetic patients show a significantly higher mean glucose concentration ($142.3 \text{ mg/dL}$) compared to non-diabetic patients ($110.0 \text{ mg/dL}$), reflecting a $+32.3 \text{ mg/dL}$ disparity[cite: 8].
* **Body Mass Index (BMI) Drives Risk ($r \approx +0.29, p < 0.0001$):**[cite: 7, 8]
  The average BMI of diabetic subjects ($35.4 \text{ kg/m}^2$) falls into **Class II Obesity**, whereas the non-diabetic cohort mean is $30.3 \text{ kg/m}^2$ ($+5.1 \text{ kg/m}^2$ difference)[cite: 8].
* **Age-Glucose Regression Trend ($p < 0.001$):**[cite: 6]
  Linear regression models indicate that fasting glucose rises by approximately **$0.72 \text{ mg/dL}$ per additional year of age** ($\text{Glucose} \approx 97.08 + 0.7164 \times \text{Age}$), with age explaining $\approx 7.2\%$ of total variance in glucose levels[cite: 6].
* **Hypothesis Testing Summary:** Welch's $t$-tests confirm that Glucose, BMI, and Age show statistically significant differences between diabetic and non-diabetic groups ($p < 0.0001$ for all three variables)[cite: 8].

---

## 📂 Repository Structure

├── Pima_Indians_Diabetes_Analysis.ipynb  # Main Jupyter/Colab notebook containing Questions 1-20
├── README.md                             # Project documentation and summary
└── requirements.txt                      # List of required Python packages

---

## 🚀 How to Run in Google Colab

1. **Open Google Colab:** Navigate to [Google Colab](https://colab.research.google.com/).
2. **Upload Notebook:** Upload `Pima_Indians_Diabetes_Analysis.ipynb` or import it from your GitHub repository.
3. **Execute Cells:** Run all cells sequentially (`Ctrl + F9` or `Runtime > Run all`).
4. **Dataset Loading:** The code automatically fetches the dataset directly from its raw source URL, requiring no local manual files upload.

---

## 🛠️ Tech Stack & Libraries

- **Language:** Python 3.x
- **Environment:** Google Colab / Jupyter Notebook
- **Data Manipulation:** `pandas`, `numpy`
- **Statistical Computing:** `scipy.stats`, `statsmodels`
- **Data Visualization:** `matplotlib`, `seaborn`
