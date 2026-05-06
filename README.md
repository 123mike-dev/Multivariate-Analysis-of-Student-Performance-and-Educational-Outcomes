# Multivariate Analysis of Student Performance

[**📊 View Interactive Report**](https://123mike-dev.github.io/Multivariate-Analysis-of-Student-Performance-and-Educational-Outcomes/) | [**📂 Project Wiki**](#) 

# Multivariate Analysis of Academic Performance
Multivariate Analysis of Academic Performance. An Actuarial Perspective on Educational Outcomes
## Project Overview
This project applies multivariate statistical techniques to the hsb2 dataset to determine how socio-economic factors and institutional types influence academic success across five core subjects.
Key MethodologiesHypothesis Testing: 
Hotelling’s $T^2$ tests for gender and school-type disparities.
Dimension Reduction: 
Principal Component Analysis (PCA) to identify "General Academic Ability" vs. "Subject Orientation."Multivariate Analysis: 
One-way and Two-way MANOVA to assess the impact of SES and Program type.Predictive Modeling: 
Random Forest Classification to identify high-performing students with 96% accuracy.
## Repository Structure
```text
/multivariate-academic-analysis
│
├── data/
│   └── hsb2.csv                # Raw student performance dataset
├── notebooks/
│   └── analysis_full.ipynb     # Complete Python analysis (PCA, MANOVA, CCA)
├── outputs/
│   ├── figures/                # Visualizations (Heatmaps, ROC curves)
│   └── report_summary.pdf      # Detailed interpretation of findings
├── requirements.txt            # Python dependencies
└── README.md                   # Project overview and instructions

## Getting Started
1. Install dependencies: `pip install -r requirements.txt`
2. Open `notebooks/analysis_full.ipynb` to view the step-by-step multivariate analysis.

## Summary of Findings

| Analysis Component | Key Statistic | Professional Interpretation |
| :--- | :--- | :--- |
| **Multivariate Normality** | Mardia's $p < 0.05$ | Non-normal distribution; analysis interpreted with robust statistical considerations. |
| **One-Sample Testing** | $T^2 = 20.88$ | Academic performance significantly exceeds hypothesized national benchmarks. |
| **Two-Sample (Gender)** | $T^2 = 48.59$ | Significant divergence in subject-level profiles between male and female students. |
| **Two-Sample (School)** | $T^2 = 3.58$ | No statistically significant difference in performance vectors between Public and Private schools. |
| **One-Way MANOVA** | Wilks' $\Lambda = 0.945$ | Program type has a marginal effect ($p = 0.052$) on the combined score vector. |
| **Two-Way MANOVA** | SES Wilks' $\Lambda = 0.854$ | **Socio-Economic Status (SES)** is the dominant factor driving academic disparities. |
| **PCA (PC1)** | $67.6\%$ Variance | Identified "General Academic Ability" as the primary latent factor across all subjects. |
| **Canonical Correlation** | $R = 0.433$ | Confirmed a strong multivariate link between home environment (SES) and academic outcomes. |
| **Predictive Modeling** | **$96\%$ Accuracy** | Random Forest model reliably classifies top-tier student performance (AUC = 0.99). |
