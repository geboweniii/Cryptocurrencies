# Cryptocurrencies

## Analysis Overview
This exercise uses unsupervised machine learning to analyze a database of cryptocurrencies and generate results including traded cryptocurrencies classified by group.
The classification report is of value to an investment bank in proposing new cryptocurrency investment portfolios to clients.
The following methods were utilized:
- preprocessing the database,
- reducing the data dimension using Principal Component Analysis,
- clustering cryptocurrencies using K-Means,
- visualizing classification results with 2D and 3D scatter plots.

## Resources
- Data Source: [crypto_data.csv](https://github.com/cedoula/Cryptocurrencies/blob/main/Resources/crypto_data.csv), [CryptoCompare](https://min-api.cryptocompare.com/data/all/coinlist)
- Software: Python 3.9, Jupyter Notebook

## Results
532 tradable cryptocurrencies remained after preprocessing and cleaning.

### Clustering Cryptocurrencies using K-Means - Elbow Curve
Unsupervised machine learning was used to identify clusters of the cryptocurrencies. The elbow curve below was produced by the K-Means method iterating on k values from 1 to 10. The best k value is 4.
![alt text](https://github.com/geboweniii/Cryptocurrencies/blob/main/Images/MOD18_Elbow.PNG)

### Visualizing Cryptocurrencies Results
#### 3D-Scatter plot with clusters
The 3-D scatter plot was obtained using the PCA algorithm to reduce the crytocurrencies dimensions to three principal components.
![alt text](https://github.com/geboweniii/Cryptocurrencies/blob/main/Images/MOD18_Class.PNG)

#### 2D-Scatter plot with clusters
The 2-D scatter plot was obtained using the PCA algorithm to reduce the crytocurrencies dimensions to two principal components. Both scatter plots show the distribution and the four clusters of cryptocurrencies.
![alt text](https://github.com/geboweniii/Cryptocurrencies/blob/main/Images/MOD18_Clusters2.PNG)

#### Tradable Cryptocurrencies Table
Most cryptocurrencies are part of class #0 and #1. The snapshot illustrates BitTorrent as the only cryptocurrency in class #2.
![alt text](https://github.com/geboweniii/Cryptocurrencies/blob/main/Images/MOD18_Trade.PNG)

#### 2D-Scatter plot with TotalCoinMined vs TotalCoinSupply
Plotting the scatter plot from two cryptocurrency features directly does not efficiently segregate the different classes. The PCA algorithm is the right method for better visualizations.
![alt text](https://github.com/geboweniii/Cryptocurrencies/blob/main/Images/MOD18_Total.PNG)

## Summary
The classification of 532 cryptocurrencies have been identified based on similarities of their features. Distinctions in each group must be analyzed to determine their performance and potential interest for the investment bank's clients.
