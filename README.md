# 🌾 Seasonal Agriculture Performance Analysis

## About the Project

This project presents a data-driven analysis of agricultural performance across different seasons.

The study focuses on the **Kharif, Rabi and Zaid** seasons and examines how agricultural outcomes vary with crop type, irrigation practices, environmental conditions, water efficiency and geographical location.

The purpose of the project is to transform raw agricultural records into meaningful information that can support better agricultural planning and decision-making.

---

## 🎯 Project Goals

The analysis was carried out with the following goals:

- Understand the structure and characteristics of the agricultural dataset.
- Clean and prepare the data for analysis.
- Identify and handle missing observations.
- Check for duplicate records.
- Investigate potential outliers.
- Study the distribution of important agricultural variables.
- Compare agricultural performance across seasons.
- Analyze crop-wise and irrigation-wise performance.
- Examine relationships between agricultural variables.
- Study regional differences in seasonal yield.
- Generate meaningful insights from the analysis.
- Provide practical recommendations based on the results.

---

## 📂 Dataset Description

The project uses a CSV-based agricultural dataset containing:

**4,000 records and 28 variables.**

The variables cover several aspects of agricultural activity, including:

- Farm information
- State
- District
- Crop
- Season
- Farm area
- Rainfall
- Temperature
- Soil moisture
- Irrigation method
- Water usage
- Fertilizer usage
- Pesticide usage
- Crop yield
- Revenue
- Production cost
- Profit
- Water efficiency
- Disease and pest risk

### Seasons

The analysis considers three agricultural seasons:

1. **Kharif**
2. **Rabi**
3. **Zaid**

---

# 🧹 Data Preparation

Before conducting the analysis, the dataset was examined and cleaned.

## Missing Data

Missing observations were found in:

- `Rainfall_mm`
- `Soil_Moisture_pct`
- `Yield_Tonnes_Ha`

Median values were used to fill the missing numerical observations.

This approach allowed the records to remain in the dataset while limiting the influence of extreme values on the imputation process.

## Duplicate Records

The dataset was checked for duplicate rows.

Duplicate observations, if present, were removed so that the same record would not influence the analysis more than once.

## Outlier Investigation

Potential outliers were examined using the **Interquartile Range (IQR)** method and boxplots.

The identified extreme observations were investigated rather than automatically removed because unusual agricultural values can represent real-world differences between farms.

---

# 📊 Exploratory Data Analysis

Several analytical techniques were used in the project.

## 1. Univariate Analysis

Individual variables were examined separately.

Examples include:

- Distribution of agricultural yield
- Frequency of observations by season

The yield distribution is strongly right-skewed, with many observations at lower yield levels and a smaller number of observations at substantially higher levels.

---

## 2. Bivariate Analysis

Pairs of variables were analyzed to understand their relationships.

Examples include:

- Season and yield
- Yield and water efficiency

The yield-versus-water-efficiency analysis shows a strong positive association.

---

## 3. Multivariate Analysis

Multiple agricultural indicators were considered together.

The analysis compares:

- Average yield
- Average profit
- Average water efficiency

across Kharif, Rabi and Zaid.

Normalization was applied so that indicators with different units could be compared visually.

---

# 🌱 Seasonal Yield Analysis

The calculated average yield for each season is approximately:

| Season | Average Yield |
|---|---:|
| Kharif | 5.63 tonnes/ha |
| Rabi | 5.04 tonnes/ha |
| Zaid | 4.64 tonnes/ha |

### Finding

Kharif records the highest average yield, while Zaid records the lowest average yield.

This indicates that agricultural productivity differs between the seasons represented in the dataset.

---

# 💰 Profitability by Season

Average profit differs substantially across the three seasons.

| Season | Average Profit |
|---|---:|
| Kharif | ₹1.79 lakh |
| Rabi | ₹87,689 |
| Zaid | -₹24,805 |

### Finding

Kharif demonstrates the strongest average profitability.

Zaid records a negative average profit, making it an important area for further investigation.

Factors such as production costs, crop choice, resource availability and market conditions may need to be examined.

---

# 🌾 Crop-Wise Analysis

The average yield of different crops was compared.

The analysis shows substantial variation between crop types.

**Sugarcane records the highest average yield in tonnes/ha in the dataset.**

However, yield alone is not sufficient to determine which crop performs best economically.

Crop selection should also consider:

- Production costs
- Revenue
- Profit
- Water requirements
- Other resource requirements

---

# 💧 Irrigation Analysis

Different irrigation methods were compared using several performance indicators.

The analysis considered:

- Average yield
- Average profit
- Water consumed
- Water efficiency

### Key Finding

Drip irrigation records an average yield of approximately:

**6.58 tonnes/ha**

It also records an average profit of approximately:

**₹2.20 lakh**

Rainfed farming records the highest water-efficiency metric at approximately:

**7.56 tonnes/1,000 m³**

These findings show that irrigation methods should be evaluated using multiple indicators rather than relying on yield alone.

---

# 💦 Water Efficiency and Yield

A scatter plot and correlation analysis were used to study the relationship between water efficiency and agricultural yield.

The calculated correlation is approximately:

**0.91**

This represents a strong positive relationship between the two variables in the dataset.

In general, observations with higher water-efficiency values tend to have higher yields.

### Important Note

A correlation does not establish causation.

Other factors, including crop type, rainfall, soil conditions, irrigation method and farming practices, may also influence yield.

---

# 🌧️ Environmental Analysis

Environmental conditions were compared between seasons.

Approximate average rainfall:

| Season | Average Rainfall |
|---|---:|
| Kharif | 849 mm |
| Rabi | 438 mm |
| Zaid | 305 mm |

### Finding

Kharif receives substantially more rainfall than Rabi and Zaid.

Zaid has the lowest average rainfall among the three seasons.

Rainfall, temperature and soil moisture therefore provide useful context when interpreting seasonal agricultural performance.

---

# 🗺️ Regional Analysis

A State × Season analysis was performed to investigate geographical differences in yield.

Some notable observations include:

- Punjab shows particularly high average yield during Rabi.
- Karnataka performs strongly during Zaid.
- Maharashtra has comparatively low Zaid yield.
- The strongest-performing season differs between some states.

This suggests that agricultural strategies should take geographical conditions into account rather than applying the same approach everywhere.

---

# 📐 Statistical Analysis

The project includes statistical techniques such as:

- Descriptive statistics
- Correlation analysis
- One-Way ANOVA
- Kruskal-Wallis test

The One-Way ANOVA produced a p-value of approximately **0.214**, which is above the 0.05 significance level.

The Kruskal-Wallis test produced a very small p-value and indicated a statistically detectable difference in the seasonal distributions/ranks.

Because the two statistical tests produce different conclusions, the seasonal patterns are interpreted carefully rather than being presented as a definitive causal effect.

---

# 💡 Major Insights

The analysis produced the following key insights:

### 1. Kharif has the highest average yield

Kharif records approximately **5.63 tonnes/ha**, higher than both Rabi and Zaid.

### 2. Zaid has the lowest average yield

Zaid records approximately **4.64 tonnes/ha**.

### 3. Kharif is the most profitable season

Kharif records an average profit of approximately **₹1.79 lakh**.

### 4. Zaid shows a profitability concern

Zaid has an average loss of approximately **₹24,805**.

### 5. Crop yields vary substantially

Sugarcane records the highest average yield in tonnes/ha among the crops analyzed.

### 6. Drip irrigation performs strongly

Drip irrigation records an average yield of approximately **6.58 tonnes/ha**.

### 7. Drip irrigation also shows high profitability

Its average profit is approximately **₹2.20 lakh**.

### 8. Rainfed farming has high water efficiency

Rainfed farming records approximately **7.56 tonnes/1,000 m³** of water efficiency.

### 9. Yield and water efficiency are strongly associated

Their correlation is approximately **0.91**.

### 10. Agricultural performance varies geographically

The State × Season analysis demonstrates that the best-performing season can differ between regions.

---

# 📌 Recommendations

Based on the findings, the following recommendations are suggested:

### Seasonal Planning

Develop separate strategies for Kharif, Rabi and Zaid based on their environmental and economic conditions.

### Improve Zaid Profitability

Investigate the reasons behind the negative average profit during Zaid.

### Efficient Irrigation

Evaluate drip irrigation where it is suitable from both an economic and operational perspective.

### Monitor Multiple Indicators

Farm performance should be evaluated using yield, profit, water efficiency, costs and risk together.

### Crop-Specific Planning

Crop selection should consider productivity as well as profitability and resource requirements.

### Regional Strategies

Agricultural recommendations should take state and regional differences into consideration.

### Weather Integration

Future analysis can incorporate historical and forecast weather information.

### Market Integration

Market prices and input costs should be incorporated into future profitability analysis.

---

# ⚠️ Limitations

This analysis has several limitations:

- The study uses only the supplied agricultural dataset.
- The dataset may not represent every agricultural region or farming system.
- Missing numerical values were handled using median imputation.
- Potential outliers were investigated but not automatically removed.
- Different crops naturally have different yield ranges.
- The data are observational, so statistical relationships should not automatically be interpreted as causal relationships.
- Agricultural prices and weather conditions can change over time.
- More years of data would provide stronger evidence for long-term trends.
- Field experiments or longitudinal studies would be useful for confirming causal relationships.

---

# 🛠️ Tools and Technologies

The project was developed using:

### Programming Language

**Python**

### Platform

**Google Colab**

### Libraries

- **Pandas** — Data manipulation and analysis
- **NumPy** — Numerical calculations
- **Matplotlib** — Data visualization
- **SciPy** — Statistical testing

---

# 📁 Repository Structure

```text
Seasonal-Agriculture-Performance-Analysis/
│
├── README.md
│
├── seasonal_agriculture_performance_dataset.csv
│
└── Seasonal_Agriculture_Performance_Analysis.ipynb
