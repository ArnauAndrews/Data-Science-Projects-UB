Access the full project at the following link: **https://rpubs.com/ArnauAndrews/1059093**

# Analyzing Small Business Clusters for each USA State: Identifying Patterns and Opportunities for Economic Growth

Author: Arnau Andrews Alés
Date: 2023-05-01

## Table of Contents
- [Problem Statement](#problem-statement)
- [Dataset](#dataset)
- [Workflow](#workflow)
- [Findings and Conclusions](#findings-and-conclusions)
- [Next Steps](#next-steps)

## Problem Statement
This project focuses on analyzing small businesses in the United States, which are crucial for economic development. The goal is to identify patterns and opportunities for economic growth among small businesses. The dataset used is obtained from the U.S. Small Business Administration (SBA), containing economic data for small businesses in each state.

## Dataset
The dataset consists of 51 observations, representing each federal state in the USA, and 16 variables related to economic data for small businesses. Missing values are represented as asterisks, which were replaced with the median for each variable. The dataset was transformed into a numeric type and standardized for further analysis.

## Workflow
1. **Dataset Preparation:**
   - Replaced missing values with the median and transformed variables into a numeric type.
   - Standardized the variables by creating a new dataframe.

2. **Cluster Creation:**

 - Estimated the optimal number of clusters using the elbow method
   
![Unknown-2](https://github.com/ArnauAndrews/Data-Analytics-Projects-Ubiqum/assets/132329252/baea6d43-f3dd-4d6e-9fbe-d1569dded26f)

   - Estimated the optimal number of clusters using the dendrogram representation.
   - 
![Unknown-3](https://github.com/ArnauAndrews/Data-Analytics-Projects-Ubiqum/assets/132329252/07f741b5-1b5b-4160-924e-7b9f0105c473)

   - Created clusters based on the chosen number using the k-means algorithm.
   - Visualized the clusters in two dimensions using the fviz_cluster function.

![Unknown-4](https://github.com/ArnauAndrews/Data-Analytics-Projects-Ubiqum/assets/132329252/d7eed412-ec3e-4f78-8a48-cf1034f9be02)

4. **Cluster Interpretation:**
   - Determined the most representative state for each cluster based on the distance to the centroid.
   - Indexed the most representative states in the initial dataframe and created a new dataset including these states.
   - Identified the variables that differed the most in value between states.
   - Determined the state with the highest unemployment rate among the selected states.

5. **Campaign Proposal:**
   - Proposed the cluster(s) for a campaign to increase exports from small businesses with the least export volume and lower export value.
   - Identified the cluster representing small businesses with higher income.

## Findings and Conclusions
- The optimal number of clusters was estimated to be between 4 and 8 based on the elbow method and dendrogram representation.
- Four clusters were created using the k-means algorithm, and the most representative states for each cluster were Illinois, District of Columbia, South Carolina, and Maine.
- The variables that differed the most in value between states were PercentExportValue, PercentSmallBiz, MedIncomeSelfEmpCorp, and AvgEmPerSmallBiz.
- The state with the highest unemployment rate among the selected states was District of Columbia.
- Cluster number 3, represented by South Carolina, was proposed for a campaign to increase exports from small businesses with the least export volume and lower export value.
- Cluster number 4, represented by District of Columbia, best represented small businesses with higher income.

## Next Steps
- Explore additional clustering algorithms, such as hierarchical clustering or DBSCAN, and evaluate their performance for this dataset.
- Incorporate more variables or external datasets related to small businesses and economic factors to enhance the analysis.
- Conduct a deeper analysis of the economic factors influencing small businesses in each cluster, such as the impact of government policies or industry trends.
- Monitor and analyze the impact of the proposed campaign on export volume and value for small businesses in the selected states, using updated data and evaluating the effectiveness of the campaign strategies.

## Insight on the k-means algorithm
The k-means algorithm is an iterative clustering algorithm that partitions data into k clusters. It works by assigning data points to the nearest centroid and updating the centroids based on the assigned data points. This process continues until convergence, where the centroids no longer change significantly or the maximum number of iterations is reached. The algorithm aims to minimize the within-cluster sum of squares, ensuring that data points within the same cluster are close together while maximizing the separation between clusters. In this project, the k-means algorithm was used to create clusters of small businesses based on their economic data, allowing for the identification of patterns and opportunities for economic growth.
