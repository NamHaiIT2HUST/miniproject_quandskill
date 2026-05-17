# Stroke Prediction Analysis (Mini-Project 5)

A complete end-to-end data preprocessing, mathematical modeling, and exploratory data analysis (EDA) pipeline for the **Stroke Prediction Dataset**.

This project was developed as part of the **AI Engineer Foundation Program** at Quanskill and demonstrates practical applications of:

- NumPy vectorized computation
- Mathematical optimization
- Probability & Linear Algebra
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Data preprocessing for Machine Learning

---

# 📌 Project Overview

According to the World Health Organization (WHO), stroke is the **2nd leading cause of death globally**, accounting for approximately **11% of total deaths** worldwide.

This project implements a structured and production-style workflow to:

- Clean and preprocess healthcare datasets
- Perform statistical and mathematical analysis
- Engineer meaningful healthcare features
- Visualize hidden data patterns
- Optimize regression parameters using Gradient Descent
- Prepare a machine-learning-ready dataset

---

# 📂 Project Structure

```text
stroke-prediction-project/
├── data/
│   ├── raw/
│   │   └── healthcare-dataset-stroke-data.csv
│   └── processed/
│       └── stroke_data_cleaned_encoded.csv
│
├── notebooks/
│   └── analysis.ipynb
│
├── src/
│   ├── numpy_tasks.py
│   ├── math_tasks.py
│   ├── pandas_tasks.py
│   └── utils.py
│
├── outputs/
│   ├── figures/
│   │   ├── loss_convergence.png
│   │   ├── q5_age_stroke_dist.png
│   │   ├── q9_correlation_heatmap.png
│   │   └── q9_glucose_boxplot.png
│   │
│   └── tables/
│
├── report/
│   └── final_report.pdf
│
├── requirements.txt
└── README.md
```

---

# 🛠️ Module Breakdown

## 📘 Module 1 — NumPy Advanced Manipulations

### ✅ Data Loading & Cleaning

- Extract numerical healthcare features:
  - `age`
  - `avg_glucose_level`
  - `bmi`
- Handle missing values using:
  - Column-wise mean imputation
- Convert data into optimized NumPy arrays

### ✅ Statistical Profiling

Implemented statistical calculations manually:

- Mean
- Median
- Standard Deviation

### ✅ Feature Scaling

Custom vectorized implementations of:

- Min-Max Scaling
- Z-score Normalization

### ✅ Principal Component Analysis (PCA)

Manual PCA implementation using:

- Covariance Matrix
- Eigenvalues & Eigenvectors
- Projection onto top 2 principal components

---

## 📗 Module 2 — Mathematics for AI

### ✅ Linear Algebra Foundations

- Matrix representation of patient profiles
- Shape analysis
- Matrix rank evaluation

### ✅ Probability & Risk Estimation

Computed:

- Prior probability:

\[
P(\text{stroke}=1)
\]

- Conditional probability:

\[
P(\text{stroke}=1 \mid \text{hypertension}=1)
\]

### ✅ Gradient Descent Optimization

Implemented Linear Regression from scratch using:

- Mean Squared Error (MSE)
- Partial derivatives
- Iterative Gradient Descent updates

### ✅ Singular Value Decomposition (SVD)

Matrix decomposition into:

- \(U\)
- \(\Sigma\)
- \(V^T\)

Used for dimensionality interpretation and latent structure analysis.

---

## 📙 Module 3 — Pandas & Exploratory Data Analysis

### ✅ Data Transformation

- Removed low-frequency anomalies
  - Example: `"Other"` gender entries
- Applied One-Hot Encoding using:
  - `drop_first=True`

### ✅ Feature Engineering

Created healthcare-derived features such as:

- `glucose_to_bmi_ratio`

Generated demographic categories:

- Age Groups
- BMI Categories (WHO Standards)

### ✅ Advanced Visualization

Generated and exported:

- Correlation Heatmaps
- Stroke Distribution Charts
- Glucose Level Boxplots
- Age Distribution Histograms

---

# 📊 Sample Outputs

Generated visualization outputs include:

| Visualization | Description |
|---|---|
| `loss_convergence.png` | Gradient Descent convergence |
| `q5_age_stroke_dist.png` | Stroke distribution by age |
| `q9_correlation_heatmap.png` | Correlation between variables |
| `q9_glucose_boxplot.png` | Glucose distribution analysis |

---

# 🚀 Getting Started

## ✅ Prerequisites

Ensure you have:

- Python 3.8+
- pip package manager

Install dependencies:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

Or install directly from:

```bash
pip install -r requirements.txt
```

---

# ▶️ Execution Pipeline

Run each module independently from the project root directory.

## Run Module 1 — NumPy Operations

```bash
python src/numpy_tasks.py
```

## Run Module 2 — Mathematics & Optimization

```bash
python src/math_tasks.py
```

## Run Module 3 — Pandas EDA & Visualization

```bash
python src/pandas_tasks.py
```

---

# 📓 Jupyter Notebook

To explore the interactive notebook:

```bash
jupyter notebook notebooks/analysis.ipynb
```

The notebook contains:

- Inline explanations
- Visual analytics
- Mathematical derivations
- Step-by-step preprocessing workflow

---

# 📈 Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

---

# 🎯 Learning Objectives

This project demonstrates understanding of:

- Vectorized numerical computation
- Statistical preprocessing
- Mathematical optimization
- Linear algebra applications
- Probability in AI
- Data visualization
- Feature engineering
- End-to-end ML preprocessing pipelines

---

# 📝 License

This project was developed for educational purposes under the **AI Engineer Foundation Program** at Quanskill.

---

# 👨‍💻 Author

AI Engineer student quandskill K9

---
