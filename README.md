# AQI Data Science Project

## Project Title
Global Urban Air Quality Index Analysis (2015–2025)

## Student Name
Farhan Rahim

## Registration Number
2280217

## Dataset Name
Global Urban Air Quality Index Dataset (2015–2025)  
File: `dataset/global_urban_aqi_dataset.csv`  
Rows: ~9,000 | Columns: 13

## Problem Statement
This project analyzes global air quality data from 2015 to 2025 across 30 major cities in 26 countries. The purpose is to understand AQI trends, identify the most influential pollutants, classify AQI categories using KNN and Naive Bayes supervised learning algorithms, and discover hidden pollution patterns using K-Means clustering and PCA.

## Tools and Libraries Used
| Library | Version | Purpose |
|---------|---------|---------|
| pandas | 3.0+ | Data loading, cleaning, manipulation |
| numpy | 2.4+ | Numerical computations |
| matplotlib | 3.10+ | Charting and visualization |
| seaborn | 0.13+ | Statistical visualizations |
| scikit-learn | 1.8+ | ML models (KNN, Naive Bayes, K-Means, PCA) |
| nbformat | 5.10+ | Notebook creation |

## How to Run the Notebook
```bash
# 1. Clone the repository
git clone https://github.com/farhanrahim160/AQI-Data-Science-Project.git
cd AQI-Data-Science-Project

# 2. Install dependencies
pip install -r requirements.txt

# 3. Launch Jupyter
jupyter notebook notebook/AQI_Data_Science_Project.ipynb
```
> **Note:** Run cells from top to bottom. The notebook creates output folders automatically.

## Summary of Main Findings
- **Highest AQI countries:** Bangladesh, Pakistan, India, and China show average AQI consistently above 150 (Unhealthy).
- **Lowest AQI countries:** Sweden, Australia, Canada, and Germany average below 60 (Good/Moderate).
- **Key pollutant:** PM2.5 has the strongest linear correlation with AQI (Pearson r ≈ 0.95+).
- **Best classifier:** KNN (k=5 or k=7) outperforms Gaussian Naive Bayes due to correlated features.
- **K-Means clusters:** Three distinct pollution groups (Low / Medium / High) were recovered without using labels.
- **PCA:** Two principal components explain significant variance; PC1 captures pollution intensity, PC2 captures weather effects.

## Screenshots of Important Charts
Charts are saved in `outputs/charts/` and `outputs/results/`:
- `chart1_aqi_distribution.png` – AQI category bar chart
- `chart2_avg_aqi_country.png` – Country-level AQI comparison
- `chart3_aqi_trend_year.png` – Yearly AQI trend
- `chart4_pm25_vs_aqi.png` – PM2.5 vs AQI scatter
- `chart5_correlation_heatmap.png` – Feature correlation heatmap
- `knn_confusion_matrix.png` – KNN confusion matrix
- `nb_confusion_matrix.png` – Naive Bayes confusion matrix
- `kmeans_clusters.png` – K-Means cluster summaries
- `pca_visualization.png` – PCA 2D scatter plot

## Report File Location
`report/AQI_Data_Science_Report.pdf`

## AI Tool Usage
This project was developed with the assistance of **Claude AI (Anthropic)** for code generation and notebook structuring. All results and written interpretations represent the student's own analysis.
