# 🌾 Assessing Australia's Agricultural Sustainability in the Context of Global Climate Change Indicators

## 📌 Overview

This project explores the sustainability of Australia's agricultural sector amidst the challenges of global climate change. Through statistical modeling and data analysis, it aims to reveal the most influential environmental factors and Australia's position relative to other nations in terms of agricultural sustainability.

---

## 🎯 Objectives

- Evaluate Australia's agricultural sustainability using global climate indicators.
- Perform statistical analysis and visualizations to explore key relationships.
- Use clustering and dimensionality reduction to classify and interpret results.
- Provide insight for future sustainability strategies.

---

## 🗂️ Dataset

- **Source:** [World Bank Group](https://data.worldbank.org/)
- **Type:** Cross-sectional
- **Period:** Most recent data available from 2001–2020
- **Rows:** 217 countries  
- **Columns:** 79 climate and agricultural indicators

---

## 📊 Key Indicators

- Agricultural land (% of total area)
- Arable land (%)
- Irrigated land (%)
- Cereal yield (kg/ha)
- CO₂ and GHG emissions
- Access to renewable energy
- Disaster risk indicators

---

## 🛠️ Tools & Technologies

- **Language:** R
- **Libraries Used:**
  - `tidyverse`
  - `ggplot2`
  - `naniar`
  - `mice`
  - `dplyr`
  - `corrplot`
  - `cluster`
  - `factoextra`

---

## 🧹 Data Preprocessing

- Identified and handled missing values.
- Imputed numeric missing values with the **mean** (excluding key response variables).
- Converted integer columns to numeric using a custom `convertToNum()` function.
- Removed rows with missing values in critical columns:
  - `AG.LND.AGRI.ZS`
  - `AG.LND.ARBL.ZS`
  - `AG.LND.IRIG.AG.ZS`

---

## 🔬 Methodology

1. **Exploratory Data Analysis (EDA)**
2. **Regression Analysis** – to understand impact on agricultural land
3. **Principal Component Analysis (PCA)** – for dimensionality reduction
4. **K-Means Clustering** – to group countries based on sustainability features

---

## 📈 Results

- Strong correlations identified between agricultural metrics and climate variables.
- Australia placed in **Cluster 2**, indicating **moderate sustainability concerns**.
- PCA helped highlight the most influential variables.

---

## ⚠️ Limitations

- Snapshot data limits time-trend analysis.
- Mean imputation may obscure some variability.
- World Bank data gaps may affect accuracy.

---

## 🔭 Future Enhancements

- Use **time-series** data for trend analysis.
- Integrate **Australian local/regional** datasets.
- Explore **advanced imputation techniques**.

---

## 📝 Conclusion

This project demonstrates the value of climate data analysis in understanding agricultural sustainability. The insights gained could help develop informed policy decisions and adaptation strategies for Australia’s agricultural future.

---

## 📎 License

This project is for academic purposes and does not include any proprietary code or datasets.

