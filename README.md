# Content Score: Analyzing Metrics Using Principal Component Analysis

This project aims to create a single variable to measure Weather Channel content by. Utilizing a Principal Component Analysis (PCA) to determine the importance of various time-based metrics from video and article data, the goal is to identify a combination of variables and use the underlying patterns in their PCA weights to create a well defined and accurate content score.

## 📌 Purpose

The project aims to:
1. Apply PCA to video metrics data to uncover latent variables.
2. Interpret PCA weights in the context of time-based viewing patterns.
3. Test over multiple combinations of content varibales. 

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
A link to the [overview](https://docs.google.com/presentation/d/100dL1hWPIGiG7HWflo1zFf7Lb9M___xqVrMCv2woghk/edit?slide=id.g3369b4db50b_0_0#slide=id.g3369b4db50b_0_0) of my findings can be found here along with accompanying reports for the latest versions of the content scores: [V2](https://docs.google.com/presentation/d/1DwxSftw3wK3XFOZldXHD7aO3MoVp4giHdUwJxRGCKII/edit?slide=id.g3369b4db50b_0_0#slide=id.g3369b4db50b_0_0) and [A3](https://docs.google.com/presentation/d/1N6Zji6iiYgxi3fPdVmWDEtRIYmz8q_P34w5UckgDm-U/edit?slide=id.g3369b4db50b_0_0#slide=id.g3369b4db50b_0_0).

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
