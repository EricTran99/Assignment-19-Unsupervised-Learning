# Assignment-19-Unsupervised-Learning
This is a repository which explore and understand the use of unsupervised machine learning.
In the respository are two files;
- Crypto_Clustering - the main script which was edited through Panda, hvplot and sklearn from scikit
- crypto_market_data.csv - the resource data in the 'Resources' folder

<h3> Exploring the Data Result </h3>
in the dataset, it contains the most popular crypto coins and the price change across the time periods.
there are two plot predictions that occur to showcase different between predicting unsuperived and one through Principal component analysis (PCA).

the first set was determine what's the best cluster number to use, by determing the K-means.
1. the first elbow plot </br>
![image](https://github.com/Nisloen/Assignment-19-Unsupervised-Learning/assets/134130254/2118f12e-826d-475d-9a79-ea7492c7c79f)

2. the pca elbow plot </br>
![image](https://github.com/Nisloen/Assignment-19-Unsupervised-Learning/assets/134130254/ec5fc50a-25db-4ad5-ad10-1dd9b8bf8c87)

By looking at the two plots, there's little differences and the ideal K-mean value is 4. Howver, when the detemine value is implemented to plot the clusters,
the results shows at the bottom.

1. the first cluster plot </br>
![image](https://github.com/Nisloen/Assignment-19-Unsupervised-Learning/assets/134130254/68b6b285-8c22-4702-b738-9681e114531c)

2. the pca cluster plot </br>
![image](https://github.com/Nisloen/Assignment-19-Unsupervised-Learning/assets/134130254/d52c1b80-ed2f-42a2-93bf-f5aefeb79465)

As the two cluster results shows, there is a significant impact.
