<!-- Project Title -->
# 🚗 Predicting 1/4 Mile Time (`qsec`) from Car Specifications

![R](https://img.shields.io/badge/Built%20with-R-blue?logo=R&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green.svg)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

---

## 📊 Overview

This repository contains R code and analysis to predict the **1/4 mile time (`qsec`)** of vehicles based on various car specifications using the `mtcars` dataset. Several linear regression models were explored — including interaction terms, quadratic terms, and Box-Cox transformations — to determine the most statistically significant model for accurate predictions.

---

## 📁 Project Structure

📦 qsec-prediction
├── 📜 README.md
├── 📊 qsec_regression.R
├── 📈 boxcox_analysis.png
└── 📁 output/
├── 📄 summary_fit1.txt
└── 📄 summary_fit2.txt


---

## 📌 Key Features

- ✅ Multiple Linear Regression Models
- 🔍 Comparison between models with interaction and quadratic terms
- 🧪 ANOVA for model significance
- 📦 Box-Cox transformation to improve model accuracy
- 📈 Visual insights into lambda selection and model diagnostics

---

## 📊 Results Summary

| Model | Adjusted R² | Residual Std. Error | p-value (F-test) | Notes |
|-------|-------------|----------------------|------------------|-------|
| Model 1 | **0.763** | 0.950 | `4.65e-05` | Interaction terms only |
| Model 2 | 0.720 | 0.946 | `5.75e-05` | Quadratic terms only |
| Model 3 (`fit2`) | 0.7106 | 0.961 | `1.889e-06` | Best fit with significant terms |

---

## 🧪 Methodology

1. **Initial Modeling**:
   - Linear regression with main effects.
2. **Model Comparison**:
   - Using ANOVA to compare interaction vs. polynomial models.
3. **Model Simplification**:
   - Removing non-significant terms.
4. **Transformation**:
   - Applied Box-Cox to check for potential improvement.

---

## 📦 Dependencies

```r
library(MASS)
library(car)

📸 Visuals
<img src="output/boxcox_analysis.png" alt="Box-Cox Plot" width="500"/>

## 🧠 Author  
**Charan Bokka**  
Master of Science in Industrial Engineering | Texas Tech University  
🔗 [LinkedIn](https://www.linkedin.com/in/charan28)  
📧 [charannb3@gmail.com]  

📜 License
This project is licensed under the MIT License - see the LICENSE file for details.


---

Let me know if you want this styled for a data science portfolio, to include binder links or Shiny apps, or if you'd like the `README` in a downloadable `.md` file format.


