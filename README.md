# Cryptocurrency Clustering Project

## Overview

This project focuses on using unsupervised learning, specifically the K-Means clustering algorithm, to analyze and cluster cryptocurrencies based on their price change percentages over different time intervals. The project includes data preprocessing, exploratory data analysis, and the application of dimensionality reduction techniques such as Principal Component Analysis (PCA).

## Project Structure

- `crypto_clustering.ipynb`: Jupyter Notebook containing the main project code.
- `Resources/`: Folder containing the dataset (`crypto_market_data.csv`).
- `README.md`: Project documentation and instructions.

## Project Requirements

- Python 3.x
- Jupyter Notebook
- Required Python libraries: pandas, hvplot, scikit-learn

## How to Run

1. Clone the repository to your local machine:

```bash
git clone https://github.com/your-username/crypto-clustering.git

###Data Preparation:
- Normalize the data using the StandardScaler module.
- Create a DataFrame with the scaled data.
- Set the coin_id column as the index.

###Find the Best Value for k (Original Data):
- Use the elbow method to determine the optimal number of clusters.
- Plot the elbow curve and identify the best value for k.

###Cluster Cryptocurrencies with K-Means (Original Data):
- Initialize and fit the K-Means model with the best value for k.
- Predict clusters and add a new column with the predicted clusters.
- Create a scatter plot using hvPlot to visualize the clusters.

###Optimize Clusters with PCA:
- Perform Principal Component Analysis to reduce features to three principal components.
- Determine the total explained variance.
- Create a new DataFrame with PCA data.

###Find the Best Value for k (PCA Data):
- Use the elbow method on PCA data to find the best value for k.
- Plot the elbow curve and identify the best value for k.

###Cluster Cryptocurrencies with K-Means (PCA Data):
- Initialize and fit the K-Means model with the best value for k using PCA data.
- Predict clusters and add a new column with the predicted clusters.
- Create a scatter plot using hvPlot to visualize the clusters.

###Visualize and Compare the Results:
Create composite plots to contrast elbow curves and cluster plots.

##Conclusion
This project provides insights into clustering cryptocurrencies based on price change percentages. The use of PCA is explored to understand the impact of dimensionality reduction on clustering performance.
