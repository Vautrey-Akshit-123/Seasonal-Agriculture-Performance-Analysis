# 🌾 Seasonal Agriculture Performance Analysis

A data analytics project investigating how agricultural performance — yield, profitability, resource usage, and risk — varies across seasons in India, using a 4,000-record farm-level dataset spanning three seasons, eight crops, eight states, and four irrigation methods.

---

## 📌 Problem Statement

Agricultural activities are influenced by seasonal variations in environmental conditions, farming practices, resource availability and market conditions. As a result, agricultural performance may differ from one season to another.

However, raw agricultural data does not clearly explain *how* performance changes across seasons or *what patterns* can be observed in different seasonal conditions.

**This project analyzes a seasonal agriculture dataset to investigate seasonal differences in agricultural performance by identifying meaningful patterns, trends, relationships and variations within the available data.**

---

## 🎯 Objective

- Explore and understand the dataset
- Clean and prepare the data for analysis
- Examine how agricultural performance varies across seasons (Kharif, Rabi, Zaid)
- Identify important seasonal patterns and trends
- Investigate relationships between seasonal conditions and agricultural outcomes
- Compare relevant groups (crop, irrigation method, region) within different seasons
- Identify significant differences or unusual patterns
- Apply appropriate statistical and visualization techniques
- Develop evidence-based, data-driven recommendations

---

## 📂 Dataset Overview

| Detail | Description |
|---|---|
| Records | 4,000 farm-level observations |
| Variables | 28 columns |
| Seasons | Kharif, Rabi, Zaid |
| Crops | Wheat, Maize, Pulses, Rice, Cotton, Chilli, Groundnut, Sugarcane |
| Irrigation Methods | Drip, Sprinkler, Flood, Rainfed |
| Categories | Location (State, District), Environmental (rainfall, temperature, humidity, soil), Farming inputs (fertilizer, pesticide, seed quality), Production (yield, water efficiency), Economic (cost, revenue, profit) |

---

## 🛠️ Tech Stack

- **Language:** Python
- **Data Handling:** Pandas, NumPy
- **Visualization:** Matplotlib, Seaborn
- **Environment:** Jupyter Notebook / Google Colab
- **Techniques:** Descriptive statistics, IQR-based outlier detection, correlation analysis, univariate/bivariate/multivariate analysis, groupby-based seasonal & regional comparisons

---

## 🔍 Analysis Workflow

1. Data loading and structural overview (shape, dtypes, head)
2. Data quality checks — missing values, duplicates, cleaning justification
3. Feature review and variable classification
4. Descriptive statistical analysis by season
5. Univariate analysis (distributions of yield, profit, season, crop)
6. Outlier analysis using the IQR method
7. Bivariate analysis (season vs. yield/profit, rainfall vs. yield, irrigation vs. yield)
8. Multivariate analysis and full correlation matrix
9. Seasonal comparison tables and visualizations
10. Additional student-driven analyses (regional differences, water efficiency by irrigation × season, disease/pest risk vs. profit)
11. Key insights, recommendations, and conclusion

---

## 📊 Key Findings

- **Crop selection drives profitability more consistently than season.** Sugarcane and Chilli stay profitable in *every* season; Wheat, Rice and Maize post negative average profit in *every* season.
- **Drip irrigation delivers the highest average yield** (~6.6 t/ha) among all irrigation methods, followed by Sprinkler, Flood, and Rainfed.
- **Zaid is the only season with negative total profit**, despite only a modest yield disadvantage compared to Kharif and Rabi — cost and price pressures compound sharply in this season.
- **Yield is highly right-skewed**, dominated by Sugarcane's scale — most "overall" statistics are more meaningful when read per crop or via the median.
- **Revenue explains profit more strongly than yield does** (r = 0.89 vs. r = 0.49) — a high-yield outcome does not guarantee a high-profit one.
- **Wet-season conditions (rainfall, humidity) correlate with higher disease/pest risk** (r = 0.62 and 0.55 respectively), concentrated most heavily in Kharif.
- **State-level analysis shows Punjab and Karnataka remain profitable even in the Zaid season**, unlike most other states — a promising lead for further investigation.

*(Full evidence, statistics, and interpretation for every finding are documented in the notebook.)*

---

## 💡 Recommendations

1. Prioritize crop-diversification support for Wheat/Rice/Maize growers, who are structurally disadvantaged regardless of season.
2. Focus water-subsidy and credit programs on the Zaid season, the least profitable and most irrigation-dependent period.
3. Promote Drip irrigation adoption, especially for farms currently on Flood/Rainfed methods.
4. Treat yield and profit as separate goals — advisory tools should report expected profit, not yield alone.
5. Target pest/disease management outreach at the Kharif season, when risk is highest.

---

## 🚀 Future Scope

- Predictive modeling (regression/ML) to forecast yield and profit
- Integration of real-time weather and soil-sensor data via APIs
- Multi-year analysis to study climate-driven seasonal trends
- A farmer-facing advisory dashboard for crop and irrigation recommendations
- Market-price forecasting to help farmers time sales for better revenue
- Clustering farms into performance segments for targeted intervention

---

## 📁 Repository Structure

````

├── Seasonal_Agriculture_Performance_Data_Analytics.ipynb   # Full analysis notebook
├── VOIS_Major_Project_PPT_Submission.pptx                  # Project presentation
├── seasonal_agriculture_performance_dataset                # Source dataset (CSV)
├── Major Project_Seasonal Agriculture Performance Analysis.PDF
└── README.md

````

---

## ▶️ How to Run

1. Clone the repository
````bash
   git clone https://github.com/<your-username>/<repo-name>.git
   cd <repo-name>
````

2. Install dependencies

````bash
   pip install pandas numpy matplotlib seaborn jupyter
````
3. Launch the notebook

````bash
   jupyter notebook Seasonal_Agriculture_Performance_Data_Analytics.ipynb
````

   *(or open it directly in Google Colab)*

---

## ⚠️ Limitations

All relationships reported are **associations** observed in a single cross-sectional dataset of 4,000 farm records — none of the analysis establishes causation. Zaid is under-represented (594 of 4,000 records) relative to Kharif/Rabi, so its statistics carry more sampling uncertainty. Findings should be validated with domain experts before being acted on at scale.

---

## 🙋 Author

**AKSHIT VAUTREY**


AICTE VOIS Batch 2026–2027 — Major Project: Seasonal Agriculture Performance Analysis



