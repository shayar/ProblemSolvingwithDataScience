# 🌍 Life Expectancy Prediction (WHO Dataset)

**Authors:** Melvin Gurung & Shayar Shrestha

---

## 📌 Problem Statement

Predicting life expectancy is crucial for global public health planning. This project analyzes and models the life expectancy of countries worldwide based on socioeconomic, health, and demographic indicators using WHO data.

**Key Questions:**

- Which factors significantly influence life expectancy?

---

## 📊 Data

- **Source:** [Kaggle: WHO Life Expectancy Data](https://www.kaggle.com/datasets/kumarajarshi/life-expectancy-who)
- **File:** `Life Expectancy Data.csv`

---

## 🛠️ Solution Overview

This project follows a full data science pipeline in R:

1. **Data Acquisition:** Load and inspect the raw WHO dataset.
2. **Exploratory Data Analysis (EDA):** Visualize distributions, missing values, and variable importance.
3. **Data Cleaning:** Handle missing values using median imputation and country/year-based strategies.
4. **Feature Engineering:** Identify and process numerical and categorical variables.
5. **Model Training:** Linear Regression with stepwise model selection.
6. **Model Evaluation:** Assess performance using RMSE, MAE, R², and residual plots.
7. **Interpretation & Insights:** Understand drivers of life expectancy.

---

## 📂 Folder Structure

```
LifeExpectancyPrediction/
│
├── Life Expectancy Data.csv   # Source dataset
├── Life Expectancy.Rmd        # Main R Markdown analysis
├── Life Expectancy.Rproj      # RStudio project file
├── Life Expectancy.nb.html    # Rendered HTML notebook
└── README.md                  # Project documentation
```

---

## 🚀 Technologies Used

- **Language:** R & RStudio
- **Libraries:**
  - `ggplot2`, `dplyr` (Visualization & data wrangling)
  - `caret`, `MASS`, `car`, `Metrics` (Modeling & evaluation)

---

## 🟢 How to Run

1. Clone or download the repository.
2. Open `Life Expectancy.Rproj` in RStudio.
3. Open and run `Life Expectancy.Rmd` step by step.
4. Ensure `Life Expectancy Data.csv` is present in the project directory.
5. For a quick review, see the rendered HTML: `Life Expectancy.nb.html`.

---

## 📝 Solution Workflow

1. **Setting up Libraries:** All required R packages are installed and loaded at the top of the Rmd file.
2. **Data Acquisition:** Load and preview the WHO dataset.
3. **EDA:** Visualize missing values, distributions, and relationships.
4. **Data Cleaning & Imputation:**
   - ≤5% missing: impute with median
   - > 5% missing: impute by country median, then by year
5. **Model Training:** Linear regression with all predictors, refined by stepwise selection (`stepAIC`).
6. **Model Evaluation & Diagnostics:**
   - Metrics: RMSE, MAE, R² (train/test split)
   - Residual analysis for bias/outliers
   - Cross-validation encouraged
7. **Conclusion:** Final model explains 94% of variance (test set R² = 0.94), average error ≈ 2 years. Key predictors: country, year, adult mortality, HIV/AIDS, under-five deaths, schooling.

---

## 📈 Results Summary

- **Test RMSE:** 2.30
- **Test MAE:** 1.34
- **Test R²:** 0.94

**Strengths:** High accuracy, interpretable drivers, extensive EDA  
**Limitations:** Some outlier countries, possible overfitting to country effects

---

## 🤝 Contributors

- Shayar Shrestha
- Melvin Gurung

---

## 📫 Contact

- Shayar's Email: shayarshrestha7@gmail.com,
- Shayar's LinkedIn: [[Linkedin](https://www.linkedin.com/in/shayarshrestha/)]
- Melvin's Email: melvcoded@gmail.com
- Melvin's LinkedIn: [[Linkedin](https://www.linkedin.com/in/melvin-gurung-734b55211/)]

---

## 📜 License

This project is open-source under the MIT License.

> _For educational and research purposes, exploring global health analytics using open data and R._
