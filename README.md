# Data Mining: PCA, Clustering & Classification

This repository presents an applied **data mining project** focused on analysing crime patterns in London using **dimensionality reduction, clustering techniques and classification models**.  
The project is based on real-world public data and follows a full analytical workflow, from exploratory analysis to model interpretation.

The work is part of my academic training in **Data Science Engineering** and is aligned with my professional activity as a **Data Analyst / Business Intelligence specialist**.

---

## Project Objectives

- Understand the **temporal, spatial and categorical structure** of crime data in London.
- Identify **patterns and similarities** between crime categories and boroughs.
- Apply **dimensionality reduction (SVD/PCA)** to reveal latent structures.
- Segment observations using **unsupervised clustering techniques**.
- Validate clustering quality through **silhouette analysis**.
- Build an **interpretable classification model** to distinguish crime intensity levels.

---

## Data Overview

- **Geographical scope:** London boroughs  
- **Time span:** 2012 – 2022  
- **Granularity:** Monthly aggregated crime counts  
- **Crime typology:** Major crime categories (theft, violence, drugs, robbery, etc.)

All data used are public, anonymised, and processed for academic and analytical purposes.

---

## Methodology

### 1. Exploratory Data Analysis (EDA)
- Distribution analysis of crime counts (log-scale due to skewness)
- Temporal evolution of total crime in London
- Borough-level comparisons for the most active areas
- Heatmap of crime distribution by borough and category

### 2. Dimensionality Reduction
- Singular Value Decomposition (SVD) applied to the crime-category matrix
- Projection of crime categories onto the first two components
- Interpretation of latent dimensions capturing the main variance structure

### 3. Clustering Analysis
- **K-means** clustering with optimal *k* selection via the elbow method
- **PAM (k-medoids)** and **k-medians** as robust alternatives
- **OPTICS** for density-based clustering comparison
- Internal validation using **silhouette width**

### 4. Classification & Interpretability
- Construction of a **decision tree** to classify crime intensity (Low vs High)
- Simple rule-based model for interpretability and business understanding

---

## Key Visual Outputs

The following figures summarise the main analytical steps and results:

### Exploratory Analysis & Structure
- `time_series_total_crime_london_2012_2022.png`
- `top_boroughs_crime_trends.png`
- `crime_distribution_by_category_log_scale.png`
- `crime_heatmap_borough_category.png`
- `svd_crime_categories_projection.png`

### Clustering & Modelling
- `kmeans_elbow_method_wss.png`
- `silhouette_analysis_k_selection.png`
- `final_clustering_silhouette_plot.png`
- `optics_reachability_plot.png`
- `decision_tree_crime_intensity_classification.png`

All visuals are reproducible from the original analysis and included for clarity and interpretation.

---

## Main Insights

- Crime data show **strong temporal patterns**, including a clear disruption during the COVID-19 period.
- A small number of boroughs concentrate a disproportionate share of total crime.
- The first two SVD components capture a **substantial proportion of the variance**, justifying low-dimensional representations.
- Clustering reveals **meaningful groupings**, though with moderate silhouette scores, reflecting the inherent complexity of social data.
- Simple classification rules can effectively separate **low- and high-intensity crime profiles**, supporting interpretability.

---

## Tools & Technologies

- **R** (data manipulation, visualisation, modelling)
- **SVD / PCA**
- **Clustering:** K-means, PAM, k-medians, OPTICS
- **Validation:** Silhouette analysis
- **Classification:** Decision trees
- **Visualisation:** ggplot2 and base R

---

## Context

This project was developed as part of my academic coursework in **Data Mining**, while simultaneously reflecting my practical approach to real-world analytics through **Ben&Co Business Intelligence**.

The focus is not only on technical correctness, but also on:
- interpretability,
- analytical reasoning,
- and alignment with real business or policy questions.

---

## Author

**Bencomo Vega**  
Data Analyst | Business Intelligence  

- GitHub: https://github.com/BencomoVega  
- LinkedIn: https://www.linkedin.com/in/bencomo-vega/  

---

## Licence

This project is licensed under the MIT License.
