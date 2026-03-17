# Interpretable-Clustering-Study
Passen die entdeckten Cluster im Datensatz Kundensegmentierung bei Online-Einzelhandels-Transaktionen zu einer interpretierbaren Struktur? Können wir die Bedeutung der unüberwachten Cluster erklären und validieren?

# 🛍️ Customer Segmentation Dataset

A comprehensive customer segmentation analysis using clustering algorithms to identify distinct customer groups based on behavioral and demographic features.

## 📁 Repository Structure
```
├── Customer Segmentation Dataset....csv  # Raw dataset
├── cluster_detailed_descriptions.csv     # Detailed cluster descriptions
├── cluster_means_absolute.csv            # Absolute mean values per cluster
├── cluster_means_relative.csv            # Relative mean values per cluster
├── cluster_melted_data.csv               # Melted/long-format cluster data
├── cluster_normalized_data.csv           # Normalized input features
├── cluster_optimization_metrics.csv      # Elbow/Silhouette optimization scores
├── cluster_statistics_complete.csv       # Full statistical summary per cluster
├── cluster_statistics_extended.csv       # Extended statistics with percentiles
└── cluster_summary_means.csv             # High-level cluster summary
```

## 📊 Project Overview

This project applies unsupervised machine learning to segment customers into meaningful groups. The pipeline includes:

- **Data Preprocessing** – Normalization and feature engineering
- **Cluster Optimization** – Elbow method & Silhouette score analysis
- **Cluster Profiling** – Statistical descriptions of each segment
- **Export** – Results stored in structured CSV files for further analysis

## 🔍 Key Files Explained

| File | Description |
|------|-------------|
| `cluster_optimization_metrics.csv` | Used to determine the optimal number of clusters |
| `cluster_normalized_data.csv` | Scaled features fed into the clustering model |
| `cluster_means_absolute.csv` | Raw average feature values per cluster |
| `cluster_means_relative.csv` | Feature values relative to the overall mean |
| `cluster_statistics_complete.csv` | Full stats (mean, std, min, max) per cluster |
| `cluster_detailed_descriptions.csv` | Human-readable segment descriptions |

## 🚀 Getting Started
```python
import pandas as pd

# Load cluster summary
df = pd.read_csv("cluster_summary_means.csv")
print(df.head())
```

## 🛠️ Requirements
```
pandas
numpy
scikit-learn
matplotlib
seaborn
```

Install via:
```bash
pip install -r requirements.txt
```

## 📈 Results

The analysis identified distinct customer segments, each with unique purchasing patterns and demographic profiles. See `cluster_detailed_descriptions.csv` for full segment profiles.

## 📄 License

See [LICENSE](LICENSE) for details.
