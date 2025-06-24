# Content Score: Analyzing Metrics Using Principal Component Analysis

This project explores the use of Principal Component Analysis (PCA) to analyze time-based metrics from video data. The goal is to identify underlying patterns in video viewing behavior using PCA weights.

## 📌 Purpose

The project aims to:
1. Apply PCA to video metrics data to uncover latent variables.
2. Interpret PCA weights in the context of time-based viewing patterns.

## 🔬 Research Foundation
The project uses the standard PCA implementation from scikit-learn, applying it to cleaned and standardized video metrics data. PCA is used to reduce dimensionality and understand the relative importance of each time-based feature in influencing overall video engagement.

## 🧪 Methodology
- **Data Ingestion:** Parses video metrics data (skipping the first three rows of metadata).
- **Data Cleaning:** Renames columns and strips whitespace and quotes.
- **Data Standardization:** Applies z-score normalization using StandardScaler.
- **PCA Analysis:** Computes PCA components using scikit-learn’s PCA module and interprets the sign and magnitude of the component weights.
- **Interpretation:** Discusses why some PCA weights may be negative and what that means for understanding viewing patterns.

## 📈 Results
- PCA reveals which time-based metrics contribute most to variance in video engagement.
- The sign (positive/negative) of PCA weights shows how each feature relates to the principal component—some features may be inversely correlated with the main component.

## 📚 Report
The notebook itself documents the full analysis, including data cleaning, PCA execution, and interpretation. Further analysis and discussion are provided within the notebook.

## 📂 Repository Structure
- `PCA V1.ipynb`: Jupyter Notebook code and analysis for PCA of V1 of Content Score.
- `PCA V2.ipynb`: Jupyter Notebook code and analysis for PCA of V2 of Content Score.
- `PCA A2.ipynb`: Jupyter Notebook code and analysis for PCA of A2 of Content Score.
- `PCA A3.ipynb`: Jupyter Notebook code and analysis for PCA of A3 of Content Score.
- `requirements.txt`: Python dependencies.

## 🔧 Requirements
Install dependencies using:
```bash
pip install -r requirements.txt
