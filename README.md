# 🌾 Seasonal Agriculture Performance Analysis
### **Major Data Analytics Project | VOIS Internship Program**

[![Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/downloads/)
[![Libraries](https://img.shields.io/badge/libraries-Pandas%20%7C%20NumPy%20%7C%20Matplotlib%20%7C%20Seaborn%20%7C%20SciPy-orange.svg)]()
[![License](https://img.shields.io/badge/license-MIT-green.svg)]()

---

## 📖 Project Overview
Agricultural activities in India are governed by distinct seasonal cycles (**Kharif**, **Rabi**, and **Zaid**), leading to pronounced variations in weather conditions, resource requirements, and economic returns. 

This project performs an end-to-end data analytics and statistical exploration of **4,000 farm records** across **8 Indian states** and **10 agricultural districts**, analyzing **28 agronomic, environmental, and financial variables**.

---

## 🎯 Key Objectives
1. **Data Quality & Preprocessing:** Audit 4,000 records, address missing values in physical variables (`Rainfall_mm`, `Soil_Moisture_pct`, `Yield_Tonnes_Ha`) via robust median imputation, and profile 1.5×IQR outliers.
2. **Exploratory Data Analysis (EDA):** Conduct univariate, bivariate, and multivariate analyses exploring relationships between climate factors, farm area, irrigation techniques, crop yields, and profitability.
3. **Structured Seasonal Comparisons:** Contrast Kharif, Rabi, and Zaid performance across productivity, water consumption, and economic margins.
4. **Inferential Hypothesis Testing:** Execute non-parametric statistical tests (Kruskal-Wallis H-tests, Chi-Square contingency, Spearman rank correlation) to evaluate the statistical significance of seasonal variations.
5. **Actionable Recommendations:** Provide evidence-backed strategies for farmers, FPOs, agronomists, and policymakers.

---

## 📁 Repository Structure

```
├── Seasonal_Agriculture_Performance_Data_Analytics.ipynb   # Complete, clean Jupyter/Colab notebook (38 cells)
├── VOIS_Major_Project_PPT_Submission_Template.pptx          # Complete 14-slide presentation with embedded charts
├── seasonal_agriculture_performance_dataset.csv            # 4,000-row agricultural dataset (28 features)
├── Major Project_Seasonal Agriculture Performance Analysis..pdf # Project guidelines and documentation
└── README.md                                               # Detailed project documentation & summary
```

---

## 📊 Summary of Key Findings

### 1. Seasonal Performance Hierarchy
| Metric | Kharif (Monsoon) | Rabi (Winter) | Zaid (Summer) |
| :--- | :---: | :---: | :---: |
| **Average Yield (t/ha)** | **5.63** (Peak) | **5.04** | **4.64** |
| **Average Net Profit (INR)** | **+₹178,914** | **+₹87,689** | **-₹24,804** (Deficit) |
| **Profitable Farms (%)** | **57.79%** | **48.86%** | **35.52%** |
| **Average Rainfall (mm)** | **849.2 mm** | **437.6 mm** | **304.7 mm** |
| **Average Water Used (m³)** | **6,102 m³** | **5,847 m³** | **6,420 m³** (Highest) |
| **Water Efficiency (t/1000m³)**| **5.89** | **5.19** | **4.41** |
| **Disease/Pest Risk (%)** | **54.47%** (Highest) | **40.48%** | **38.22%** |

* **Kharif** is the most profitable season, leveraging monsoon rains to boost natural water efficiency.
* **Rabi** delivers stable, reliable output under mild winter temperatures (23.5°C).
* **Zaid** is a critical financial stress period with negative average margins due to intense heat (31.0°C) and heavy artificial irrigation demand.

---

### 2. Statistical Hypothesis Testing Outcomes
* **Yield Across Seasons (Kruskal-Wallis):** $H = 68.71,\; p = 1.20 \times 10^{-15}$ $\rightarrow$ **Statistically Significant difference**.
* **Profit Across Seasons (Kruskal-Wallis):** $H = 101.93,\; p = 7.36 \times 10^{-23}$ $\rightarrow$ **Statistically Significant difference**.
* **Irrigation Method vs. Season (Chi-Square):** $\chi^2 = 3.51,\; p = 0.7423$ $\rightarrow$ Irrigation method choice is currently uniform across seasons, indicating an opportunity for targeted micro-irrigation modernization.
* **Rainfall vs. Yield (Spearman Rank Correlation):** $\rho = 0.1298,\; p = 1.70 \times 10^{-16}$ $\rightarrow$ Statistically significant positive correlation.

---

### 3. Top & Bottom Performing Combinations
* **Top 5 Profitable:** Sugarcane (Kharif: +₹1.00M), Chilli (Kharif: +₹954k), Sugarcane (Rabi: +₹732k), Chilli (Rabi: +₹639k), Sugarcane (Zaid: +₹584k).
* **Bottom 5 Least Profitable:** Rice (Zaid: -₹227k), Maize (Zaid: -₹194k), Wheat (Zaid: -₹193k), Pulses (Zaid: -₹139k), Wheat (Rabi: -₹120k).

---

## 🚀 How to Run the Project

### Option A: Google Colab (One-Click Execution)
1. Open [Google Colab](https://colab.research.google.com/).
2. Click **File** $\rightarrow$ **Upload notebook** $\rightarrow$ select `Seasonal_Agriculture_Performance_Data_Analytics.ipynb`.
3. Click **Runtime** $\rightarrow$ **Run all** (`Ctrl+F9` / `Cmd+F9`).
> *The notebook includes an automated online fallback that fetches the dataset directly from GitHub, requiring zero manual configuration.*

### Option B: Local Python Environment
```bash
# Clone this repository
git clone https://github.com/<your-username>/Seasonal-Agriculture-Performance-Analysis.git
cd Seasonal-Agriculture-Performance-Analysis

# Install dependencies
pip install pandas numpy matplotlib seaborn scipy jupyter

# Launch Jupyter Notebook
jupyter notebook Seasonal_Agriculture_Performance_Data_Analytics.ipynb
```

---

## 👨‍💻 Author & Acknowledgments
* **Author:** Vinit Chaurasia
* **Internship Program:** VOIS Major Data Analytics Project
* **Course Certification:** VOIS Data Visualization Course
