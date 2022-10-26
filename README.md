# Assignment 10
_________________________________________
## Project Background
_________________________________________
In this Challenge, you’ll combine your financial Python programming skills with the new unsupervised learning skills that you acquired in this module.

The CSV file provided for this challenge contains price change data of cryptocurrencies in different periods.

The steps for this challenge are broken out into the following sections:

Import the Data (provided in the starter code)
Prepare the Data (provided in the starter code)
Find the Best Value for k Using the Original Data
Cluster Cryptocurrencies with K-means Using the Original Data
Optimize Clusters with Principal Component Analysis
Find the Best Value for k Using the PCA Data
Cluster the Cryptocurrencies with K-means Using the PCA Data
Visualize and Compare the Results

## Files and Sources 
crypto_market_data.csv
 
## Calculations
Original crypto market data:

Code the elbow method algorithm to find the best value for k. Use a range from 1 to 11.
Plot a line chart with all the inertia values computed with the different values of k to visually identify the optimal value for k.
Initialize the K-Means model with four clusters using the best value for k.
Fit the K-Means model using the original data.
Predict the clusters to group the cryptocurrencies using the original data. View the resulting array of cluster values.
Create a copy of the original data and add a new column with the predicted clusters.
Create a scatter plot using hvPlot by setting x="price_change_percentage_24h" and y="price_change_percentage_7d". Color the graph points with the labels found using K-Means and add the crypto name in the hover_cols parameter to identify the cryptocurrency represented by each data point.

crypto market PCA data

Create a PCA model instance and set n_components=3.
Use the PCA model to reduce to three principal components. View the first five rows of the DataFrame.
Retrieve the explained variance to determine how much information can be attributed to each principal component.
Answer the following question: What is the total explained variance of the three principal components?
Create a new DataFrame with the PCA data. Be sure to set the coin_id index from the original DataFrame as the index for the new DataFrame. Review the resulting DataFrame.
Code the elbow method algorithm and use the PCA data to find the best value for k. Use a range from 1 to 11.
Plot a line chart with all the inertia values computed with the different values of k to visually identify the optimal value for k.

Cluster Cryptocurrencies with K-means Using the PCA Data
Initialize the K-Means model with four clusters using the best value for k.
Fit the K-Means model using the PCA data.
Predict the clusters to group the cryptocurrencies using the PCA data. View the resulting array of cluster values.
Add a new column to the DataFrame with the PCA data to store the predicted clusters.
Create a scatter plot using hvPlot by setting x="PC1" and y="PC2". Color the graph points with the labels found using K-Means and add the crypto name in the hover_cols parameter to identify the cryptocurrency represented by each data point.

Visualize and Compare the Results
Create a composite plot using hvPlot and the plus (+) operator to contrast the Elbow Curve that you created to find the best value for k with the original and the PCA data.
Create a composite plot using hvPlot and the plus (+) operator to contrast the cryptocurrencies clusters using the original and the PCA data.
Answer the following question: After visually analyzing the cluster analysis results, what is the impact of using fewer features to cluster the data using K-Means?

## Conclusion of Anlysis

Question: What is the best value for k?
Answer: The best k value is 4.

Question: What is the total explained variance of the three principal components?
Answer:  88% of the total variance is condensed into the three priciple components.

Question: What is the best value for k when using the PCA data?
Answer:  The best Value for k when using PCA, is 4.

Question: Does it differ from the best k value found using the original data?
Answer:  the K value does not differ from the orginal data. It still reamins at 4.

Question: After visually analyzing the cluster analysis results, what is the impact of using fewer features to cluster the data using K-Means?
Answer:  by using few features to cluster the data, by using K-Means, we are able to output a prediction model which is much more legiblle and clarified, as pose to the conveluted original unclustered dataset.
