# CryptoClustering
An unsupervised learning  project to predict if cryptocurrencies are affected by 24-hour or 7-day price changes.

## Steps to perform
1. Load CSV file into a DataFrame
2. Get the summary statistics and plot the data to see what the data looks like before proceeding.
3. Prepare the data by using <code>StandardScaler()</code> module from <code>scikit-learn</code> to normalize the data from the CSV file.
4. Create a DataFrame with the scaled data and set the <code>"coin_id"</code> index from the original DataFrame as the index for the new DataFrame.
5. Find the best value for <code>k </code> by using the original scaled DataFrame by using the elbow method
6. Cluster cryptocurrencies with <code>K-means</code> by using the original scaled data
7. Optimize crypto clusters with Principal Component Analysis
8. Create visualization using hvPlot

## Results

From the two types of combined cluster plots above, I really don't think reducing the number of feature columns used to derive on the best K value made any difference. If you look at the elbow graphs above, the K value both points at 4. Perhaps, the original data was sufficient enough.

1. The line graph below is the original dataframe consisting of all the bitcoin
![Original line graph with bitcoins](./Resources/orig_data_line_graph.png)
2. The elbow of the original DataFrame revealed that 4 is the best k value
![Orignal data k means elbow](./Resources/orig_k_means_elbow.png)
3. PCA revealed that the k means is also 4
![PCA k means elbow](./Resources/pca_elbow.png)
4. Original and PCA'd dataset point to 4 as the most efficient value of k
![Combined elbow graphs](./Resources/combined_elbow.png)