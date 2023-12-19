# Crypto Coin cluster analysis - Unsupervised Learning

This repository explored and understand the use of unsupervised machine learning with the crypto coin as the data source. With unsupervised learning, the results are shown with the K-mean and two cluster plots; one being a normal cluster and the other incorporates Principal Component Analysis (PCA). In the respository, there are two files: <br/>
- Crypto_Clustering - the main script which was edited through Panda, hvplot and sklearn from scikit
- crypto_market_data.csv - the resource data in the 'Resources' folder

## Development Process
In the dataset, it contains the most popular crypto coins and the price change across the time periods. Across the crypto coins, the summary statistic was used to get a basic insight for each timepoint periods (the results is shown below). Due to the vast difference in range across the crypto coins when comparing the minimum and maximum values, the data was normalized with _StandardScaler()_ in order for the data to be readable for the algorithm. The normalized table can be seen below. <br/>
![image](https://github.com/EricTran99/Assignment-19-Unsupervised-Learning/assets/134130254/b14b3430-b414-411d-b7e0-dcaca920bcac) <br/>
 <br/>
![image](https://github.com/EricTran99/Assignment-19-Unsupervised-Learning/assets/134130254/676c7125-a985-4e25-95a6-3485c0d7c36c) <br/>
 <br/>
The method used for the unsupervised learning was to group the results into clusters, thus the K-mean was calculated in order to find the best amount of cluster for grouping. Additionally, the PCA was incorporated to compare the differences the results without PCA. <br/>
1. the first elbow plot </br>
![image](https://github.com/Nisloen/Assignment-19-Unsupervised-Learning/assets/134130254/2118f12e-826d-475d-9a79-ea7492c7c79f)

2. the pca elbow plot </br>
![image](https://github.com/Nisloen/Assignment-19-Unsupervised-Learning/assets/134130254/ec5fc50a-25db-4ad5-ad10-1dd9b8bf8c87)

By looking at the two plots, there's little differences and the ideal K-mean value is 4. However, when the detemined value is implemented to plot the clusters,
the results shows at the bottom. <br/>

1. the first cluster plot </br>
![image](https://github.com/Nisloen/Assignment-19-Unsupervised-Learning/assets/134130254/68b6b285-8c22-4702-b738-9681e114531c)

2. the pca cluster plot </br>
![image](https://github.com/Nisloen/Assignment-19-Unsupervised-Learning/assets/134130254/d52c1b80-ed2f-42a2-93bf-f5aefeb79465)

As the two cluster results shows, there is a significant impact. for the first cluster plot, there is one data where it is identified as a seperate cluster eventhough
it is within the group, and it also shows two seperate cluster group despite between close to each other. Compared to the PCA cluster plot, where despite showing single
seperate cluster data, at least the cluster group is accurate. This highlights one flaw in regards to using unsupervised learning, where the method for relying the algorithm is predicting the cluster without labeled values resulted in one of the vector to be considered different despite visually within one of the cluster (this is evident with the first cluster plot). But with the optimisation (PCA), the second cluster plot showed a more distinct difference in the cluster group.

# Summary
The concept of machine learning introduces one of the method, unsupervised learning. Although the benefit of creating an algorithm in finding the pattern and grouping the values into clusters, the module shows the flaws in using unsupervised learning where it struggles for some dataset that have more complex values. This flaw is evident when compared the crypto coin price change with one cluster optimising PCA, whereas the other one has no optimisation. The results shows the un-optimised cluster to be confused with one of the values identified as a different cluster. The data was normalized and was analysed to find the best number of cluster (K-mean).
