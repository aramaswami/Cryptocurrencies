# Cryptocurrencies  
I analyzed the csv data of cryptocurrencies to predict clusters and provide visualizations The raw data was organized under the following columns: CoinName, Algorithm, IsTrading, ProofType, TotalCoinsMined, and TotalCoinSupply.  

## Project outline  
I completed the following steps as part of the analysis: (1) Data Preprocessing; (2) Reducing Data Dimensions Using PCA; (3) Clustering Cryptocurrencies Using K-means; and (4) Visualizing Results.  

### Data Preprocessing  
For this step, I created a series of dataframes to import, cleanup, reorganize, and analyze the data. I documented each step in my notebook comments.  

### PCA  
I created a PCA with 3 components. The first step was to use pandas get_dummies to convert category data and then scaled the data. With the transformed data, I ran the PCA algorithms and created a new dataframe.  

### K-means
With the PCA data, I generated an 'elbow curve' to determine the k value, which turns out to be 4 or 5. I ran the K-means algorith with 4 and created the clusters. I then created a new dataframe that combined the pca columns with other columns. 

### Visualization
The first visualization is a 3-D scatter plot of the pca elements that show how the data clusters. The next is a hvplot table with selcted columns. Finally, I created a scatter plot with x-axis as "TotalCoinsMined" and y-axis as "TotalCoinSupply"

## Summary
The data shows clear clusters that are useful to understand and describe common attributes. Further analysis may be include additional components for pca, exploration of supervised models for prediction, and additional features.

