# 🩺 Pima Indians Diabetes Dataset: Statistical Analysis & Risk Factor Prediction

An evidence-based statistical analysis and exploratory data science project using the **Pima Indians Diabetes Dataset**. This project investigates key physiological risk factors for diabetes—including **Plasma Glucose**, **BMI**, **Age**, and **Insulin**—by combining descriptive statistics, inferential hypothesis testing, bivariate correlation, linear regression, and data visualization.

---

## 📌 Project Overview

The objective of this project is to apply core statistical and probabilistic concepts to healthcare data to identify significant predictors of diabetes and construct diagnostic insights.

### Core Objectives:
1. **Dataset Inspection & Cleaning:** Quantify baseline structure ($n = 768$ observations, $p = 9$ variables) and address zero-value clinical anomalies.
2. **Exploratory Data Analysis (EDA):** Visualize density distributions (KDE), scatter plot matrices, and correlation heatmaps.
3. **Inferential Hypothesis Testing:** Perform two-sample Welch’s $t$-tests to evaluate significant differences between diabetic ($\text{Outcome} = 1$) and non-diabetic ($\text{Outcome} = 0$) cohorts.
4. **Correlation & Regression Modeling:** Measure Pearson correlation coefficients and model age-dependent glucose trends using Simple Linear Regression.
5. **Statistical Synthesis:** Integrate probability theory, Central Limit Theorem (CLT) convergence, $95\%$ Confidence Intervals, and risk factor rankings into a master analytics dashboard.

---

## 📊 Key Findings & Insights

* **Plasma Glucose ($r \approx +0.47, p < 0.0001$):** Serves as the single strongest diagnostic predictor of diabetes. Diabetic patients exhibit a significantly higher mean glucose level ($142.3 \text{ mg/dL}$) compared to non-diabetic patients ($110.0 \text{ mg/dL}$).
* **Body Mass Index ($r \approx +0.29, p < 0.0001$):** Acts as the primary modifiable risk factor. The average BMI of diabetic subjects ($35.4 \text{ kg/m}^2$) falls into **Class II Obesity**.
* **Age & Regression ($p < 0.001$):** Simple linear regression demonstrates that fasting glucose increases by approximately **$0.72 \text{ mg/dL}$ per year of age** ($\text{Glucose} = 97.08 + 0.7164 \times \text{Age}$).

---

## 🛠️ Tech Stack & Dependencies

* **Language:** Python 3.x
* **Environment:** Google Colab / Jupyter Notebook
* **Data Processing:** `pandas`, `numpy`
* **Statistical Computing:** `scipy.stats`, `statsmodels`
* **Visualization:** `matplotlib`, `seaborn`

---

## 📂 Project Structure
### Short Repository Description (GitHub About Section)

> **Statistical Analysis & Exploratory Data Science on the Pima Indians Diabetes Dataset using Python & Google Colab.**
> *Features descriptive & inferential statistics, hypothesis testing (Welch's t-test), correlation matrices, linear regression, and risk factor synthesis.*

---

### Full `README.md` Template

You can copy and paste the markdown below directly into your repository's `README.md` file:

```markdown
# 🩺 Pima Indians Diabetes Dataset: Statistical Analysis & Risk Factor Prediction

An evidence-based statistical analysis and exploratory data science project using the **Pima Indians Diabetes Dataset**. This project investigates key physiological risk factors for diabetes—including **Plasma Glucose**, **BMI**, **Age**, and **Insulin**—by combining descriptive statistics, inferential hypothesis testing, bivariate correlation, linear regression, and data visualization.

---

## 📌 Project Overview

The objective of this project is to apply core statistical and probabilistic concepts to healthcare data to identify significant predictors of diabetes and construct diagnostic insights.

### Core Objectives:
1. **Dataset Inspection & Cleaning:** Quantify baseline structure ($n = 768$ observations, $p = 9$ variables) and address zero-value clinical anomalies.
2. **Exploratory Data Analysis (EDA):** Visualize density distributions (KDE), scatter plot matrices, and correlation heatmaps.
3. **Inferential Hypothesis Testing:** Perform two-sample Welch’s $t$-tests to evaluate significant differences between diabetic ($\text{Outcome} = 1$) and non-diabetic ($\text{Outcome} = 0$) cohorts.
4. **Correlation & Regression Modeling:** Measure Pearson correlation coefficients and model age-dependent glucose trends using Simple Linear Regression.
5. **Statistical Synthesis:** Integrate probability theory, Central Limit Theorem (CLT) convergence, $95\%$ Confidence Intervals, and risk factor rankings into a master analytics dashboard.

---

## 📊 Key Findings & Insights

* **Plasma Glucose ($r \approx +0.47, p < 0.0001$):** Serves as the single strongest diagnostic predictor of diabetes. Diabetic patients exhibit a significantly higher mean glucose level ($142.3 \text{ mg/dL}$) compared to non-diabetic patients ($110.0 \text{ mg/dL}$).
* **Body Mass Index ($r \approx +0.29, p < 0.0001$):** Acts as the primary modifiable risk factor. The average BMI of diabetic subjects ($35.4 \text{ kg/m}^2$) falls into **Class II Obesity**.
* **Age & Regression ($p < 0.001$):** Simple linear regression demonstrates that fasting glucose increases by approximately **$0.72 \text{ mg/dL}$ per year of age** ($\text{Glucose} = 97.08 + 0.7164 \times \text{Age}$).

---

## 🛠️ Tech Stack & Dependencies

* **Language:** Python 3.x
* **Environment:** Google Colab / Jupyter Notebook
* **Data Processing:** `pandas`, `numpy`
* **Statistical Computing:** `scipy.stats`, `statsmodels`
* **Visualization:** `matplotlib`, `seaborn`

---

## 📂 Project Structure


```

├── diabetes_analysis.ipynb   # Complete Google Colab notebook with executed code & visualizations
├── README.md                 # Project documentation and summary
└── requirements.txt          # Python package requirements

```

---

## 🔬 Analytical Pipeline Covered

1. **Dataset Structure & Data Types**
2. **Probability & Conditional Risk ($P(D \mid X)$)**
3. **Distribution & Central Limit Theorem Analysis**
4. **$95\%$ Parameter Confidence Intervals**
5. **Two-Sample Hypothesis Testing (Welch's $t$-Test)**
6. **Pearson Correlation Heatmap & Pairplots**
7. **Simple Linear Regression ($\text{Age} \rightarrow \text{Glucose}$)**
8. **Master Diagnostic Visual Dashboard**

```
