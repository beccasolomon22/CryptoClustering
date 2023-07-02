# CryptoClustering

## Sources

1. Starter Code provided in the asssignments file
2. Stack Overflow was a great help when experiencing error messages
3. I occasionally used Chat GPT to help edit code to fix errors
4. Assignment description

# Project Overview as Described in Assignment:

Use your knowledge of Python and unsupervised learning to predict if cryptocurrencies are affected by 24-hour or 7-day price changes.

#### A general overview of the data worked with
![Overview](https://github.com/beccasolomon22/CryptoClustering/blob/main/Images/Overview.png) 

## Tools Used
1. Python
2. Pandas
3. Matplotlib
4. StandardScaler
5. PCA
6. KMeans

## Original Scaled

Using the original scaled data, created an elbow curve to see what is the optimal number of clusters
![reg_elbow](https://github.com/beccasolomon22/CryptoClustering/blob/main/Images/Reg_Elbow.png)

With an optimal value of 4 clusters, used KMeans to model, fit, and predict (with the Regular Scaled Data) to group the cryptocurrencies into 4 clusters
![reg_clusters](https://github.com/beccasolomon22/CryptoClustering/blob/main/Images/Reg_Clusters.png) 

## PCA Scaled

Using the PCA scaled data, created an elbow curve to see what is the optimal number of clusters
![pca_elbow](https://github.com/beccasolomon22/CryptoClustering/blob/main/Images/PCA_Elbow.png) 

With an optimal value of 4 clusters, used KMeans to model, fit, and predict (with the PCA Scaled Data) to group the cryptocurrencies into 4 clusters
![pca_clusters](https://github.com/beccasolomon22/CryptoClustering/blob/main/Images/PCA_Clusters.png) 

## Comparison

Regular          |   PCA
:-----------------------------------------------------------------:|:-----------------------------------------------------------------:
![reg_elbow](https://github.com/beccasolomon22/CryptoClustering/blob/main/Images/Reg_Elbow.png) | ![pca_elbow](https://github.com/beccasolomon22/CryptoClustering/blob/main/Images/PCA_Elbow.png) 
:-----------------------------------------------------------------:|:-----------------------------------------------------------------:
![reg_clusters](https://github.com/beccasolomon22/CryptoClustering/blob/main/Images/Reg_Clusters.png)   | ![pca_clusters](https://github.com/beccasolomon22/CryptoClustering/blob/main/Images/PCA_Clusters.png) 

Although each uses an optimal 4 clusters, we see a stark change between the Regular and PCA clusters. With PCA we see must more definitive clusters, without as much overlap. 

EX: Cluster 2 in the Regular clusters is nestled within cluster 3. However, in the PCA clusters, cluster 2 is completely separate from cluster 3 and there is very little overlap (a small bit of overlap can be seen with clusters 0 and 3)


