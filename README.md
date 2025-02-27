# Air Quality Analysis 

## Project Overview

This project involves clustering and anomaly detection in air quality data. The analysis applies K-Means and Hierarchical clustering techniques to identify different air quality levels and detect anomalies.

## Dataset

- `AirQualityUCI.csv` - Raw air quality data.
- `AirQuality_Preprocessed.xls` - Preprocessed dataset used for analysis.

## Data Preprocessing

- Non-numeric columns (e.g., date and time) were removed.
- Missing values were replaced with the median of respective columns.
- Relevant features (pollutant levels, sensor readings) were selected.
- Standardization was applied to normalize feature values.

## Clustering Analysis

### K-Means Clustering

- The optimal number of clusters was determined using the **Elbow Method**.
- Three clusters were identified:
  1. **Good Air Quality** - Low pollutant levels.
  2. **Moderate Pollution** - Mid-range pollutant values.
  3. **Poor Air Quality** - High pollutant levels.
- Pair plots were used to visualize feature relationships within the clusters.

### Hierarchical Clustering

- A dendrogram was used to explore hierarchical relationships between data points.

## Anomaly Detection

- **PCA (Principal Component Analysis)** was used to reduce dimensionality for better visualization.
- Data points farthest from their cluster centroids were flagged as anomalies.
- **474 anomalies** were detected, which may indicate extreme pollution events or sensor errors.
- Anomalies were highlighted in red in PCA-transformed scatter plots.

## Files in This Repository

- `Analysis Code.ipynb` - Jupyter notebook with code for clustering and anomaly detection.
- `Analysis Report Week-3.docx` - Detailed report summarizing the findings.
- `AirQualityUCI.csv` - Raw dataset.
- `AirQuality_Preprocessed.xls` - Processed dataset used in analysis.
- `README.md` - This file, providing an overview of the project.

## How to Use

### Clone the Repository

To get started with this project, clone the repository using:

```sh
git clone https://github.com/RishikaRavichandran/Air-Quality-Analysis
```



### Run the Jupyter Notebook

Launch Jupyter Notebook and open `Analysis Code.ipynb` to execute the analysis:

```sh
jupyter notebook
```

## Next Steps

- Further investigation to classify anomalies as true pollution spikes or erroneous readings.
- Fine-tuning clustering parameters for improved accuracy.
- Exploring alternative anomaly detection methods.

## Author

**Rishika Ravichandran**
Data Science Intern, Sapience Edu Connect Pvt. Ltd.

---

Feel free to contribute by refining the analysis or suggesting improvements!

