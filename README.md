# Multivariate Analysis of Academic Performance
Multivariate Analysis of Academic PerformanceAn Actuarial Perspective on Educational Outcomes
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
