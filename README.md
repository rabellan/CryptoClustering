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

