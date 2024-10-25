# Heart Disease Analysis

## Project Overview
This project analyzes a dataset of medical records to identify patients at high risk of developing heart disease. The analysis utilizes various clustering techniques such as; K-means, Hierarchical Clustering, DBSCAN clustering, and Gaussian Mixture Models (GMM), to group patients based on their medical history and identify potential risk factors associated with heart disease.

## Dataset
The dataset used in this analysis is sourced from the UCI Machine Learning Repository. It contains **303 instances** with **13 attributes**.

## Analysis Steps
1. **Data Loading and Preprocessing**:
   - Loaded the heart disease dataset.
   - Checked for missing values and handled them.
   - Scaled numerical features for clustering.
   - Encoded categorical variables using one-hot encoding.

2. **(EDA)**:
   - Visualize distributions of key variables.
   - Examine correlations between features using a heatmap.

3. **Clustering Techniques**:
   - Applied K-means clustering to group patients into distinct clusters.
   - Performed Hierarchical Clustering to explore hierarchical relationships among patients.
   - Fitted Gaussian Mixture Models (GMM) to identify underlying distributions in the data.

4. **Evaluation of Clustering Performance**:
   - Calculated Silhouette Scores and Davies-Bouldin Indices for each clustering method to assess clustering quality.

5. **Visualizations**:
   - Used PCA and t-SNE to visualize clusters and gain insights into the relationships between variables.

## Results
- **K-means** showed the best performance with a Silhouette Score of **0.182** and a Davies-Bouldin Index of **1.840**.
- **Hierarchical Clustering** had a Silhouette Score of **0.151** and a Davies-Bouldin Index of **1.989**.
- **Gaussian Mixture Models (GMM)** performed poorly with a Silhouette Score of **0.083** and a Davies-Bouldin Index of **2.762**, indicating significant overlap among clusters.

## Conclusion
- K-means was the most effective clustering algorithm in identifying potential patient groups at risk for heart disease.
- Hierarchical Clustering provided moderate results but indicated some overlap in cluster membership.
- GMM did not perform well, suggesting that the assumption of Gaussian-distributed clusters may not be appropriate for this dataset.
- DBSCAN was unsuitable for this dataset as well.