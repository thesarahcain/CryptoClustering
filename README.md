# Cryptocurrency Clustering with K-Means

This project aims to cluster cryptocurrencies based on their price change percentages using K-Means clustering algorithm and Principal Component Analysis (PCA) for dimensionality reduction.
![image](https://github.com/thesarahcain/CryptoClustering/assets/148586543/2e003317-502a-446e-b707-aef5852c943a)

## Prepare the Data
- Normalize the data using `StandardScaler()` from scikit-learn.
- Create a DataFrame with the scaled data and set the "coin_id" index.
- Visualize the first five rows of the scaled DataFrame.

## Find the Best Value for k Using the Original Scaled DataFrame
- Utilize the elbow method to determine the optimal number of clusters (k).
- Plot the inertia values for different k values to identify the best value.
![image](https://github.com/thesarahcain/CryptoClustering/assets/148586543/bfdf7507-456c-4288-971a-66f7d2efab67)

## Cluster Cryptocurrencies with K-means Using the Original Scaled Data
- Initialize and fit the K-means model with the best value for k.
- Predict the clusters and add a new column with the predicted clusters to the original data.
- Visualize the clusters using a scatter plot.
![image](https://github.com/thesarahcain/CryptoClustering/assets/148586543/72409164-cccf-47d4-ad6c-6dba29bb1a02)

## Optimize Clusters with Principal Component Analysis
- Perform PCA on the original scaled DataFrame to reduce features to three principal components.
- Calculate the explained variance and answer the question: What is the total explained variance of the three principal components?
- Create a new DataFrame with PCA data.
![image](https://github.com/thesarahcain/CryptoClustering/assets/148586543/d86155cb-43ad-4b6a-aa6a-9b5ef86b84b1)

## Find the Best Value for k Using the PCA Data
- Use the elbow method on the PCA data to find the optimal k.
- Plot the inertia values and answer the question: What is the best value for k when using the PCA data? Does it differ from the best k value found using the original data?

## Cluster Cryptocurrencies with K-means Using the PCA Data
- Initialize and fit the K-means model with the best value for k using PCA data.
- Predict the clusters and visualize them using a scatter plot.
![image](https://github.com/thesarahcain/CryptoClustering/assets/148586543/dc55cc18-870e-4c10-8f67-9455e64b5bd6)

## Resources
I references the following resources to help with my code, along with help from ChatGPT: 
https://www.digitalocean.com/community/tutorials/normalize-data-in-python
https://stackoverflow.com/questions/19197715/scikit-learn-k-means-elbow-criterion
