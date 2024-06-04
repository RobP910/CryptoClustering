# CryptoClustering

### This is my attempt at writing code that takes a csv file of crypto-currencies and makes some predictions based on the data.

## Load the data into a Pandas DataFrame and make the index the "coin_id" column.
## Generate summary statistics
## Use the `StandardScaler()` module from scikit-learn to normalize the data from the CSV file
## Create a DataFrame with the scaled data
## Copy the crypto names from the original data
## Set the coinid column as index
## Create a list with the number of k-values to try
## Use a range from 1 to 11
## Create an empty list to store the inertia values
## Create a for loop to compute the inertia with each possible value of k
## Inside the loop:
  1. Create a KMeans model using the loop counter for the n_clusters
  2. Fit the model to the data using the scaled DataFrame
  3. Append the model.inertia_ to the inertia list
## Create a dictionary with the data to plot the Elbow curve
## Create a DataFrame with the data to plot the Elbow curve
## Display the DataFrame
## Plot a line chart with all the inertia values computed with 
## the different values of k to visually identify the optimal value for k.
## Initialize the K-Means model using the best value for k
## Fit the K-Means model using the scaled data
## Predict the clusters to group the cryptocurrencies using the scaled data
## View the resulting array of cluster values
## Create a copy of the DataFrame
## Create a scatter plot using Pandas plot by setting 
## `x="price_change_percentage_24h"` and `y="price_change_percentage_7d"`.
## Use "rainbow" for the color to better visualize the data.
## Plotting
## Create a PCA model instance and set `n_components=3`.
## Use the PCA model with `fit_transform` on the original scaled DataFrame to reduce to three principal components.
## Retrieve the explained variance to determine how much information can be attributed to each principal component.
## Create a new DataFrame with the PCA data.
## Note: The code for this step is provided for you
## Creating a DataFrame with the PCA data
## Copy the crypto names from the original data
## Set the coinid column as index
## Create a list with the number of k-values to try
## Use a range from 1 to 11
## Create an empty list to store the inertia values
## Create a for loop to compute the inertia with each possible value of k
## Inside the loop:
  1. Create a KMeans model using the loop counter for the n_clusters
  2. Fit the model to the data using PCA DataFrame.
  3. Append the model.inertia_ to the inertia list
## Create a dictionary with the data to plot the Elbow curve
## Create a DataFrame with the data to plot the Elbow curve
## Plot a line chart with all the inertia values computed with 
## the different values of k to visually identify the optimal value for k.
## Initialize the K-Means model using the best value for k
## Fit the K-Means model using the PCA data
## Predict the clusters to group the cryptocurrencies using the PCA data
## View the resulting array of cluster values.
## Create a copy of the DataFrame with the PCA data
## Add a new column to the DataFrame with the predicted clusters
## Create a scatter plot using hvPlot by setting `x="PCA1"` and `y="PCA2"`. 
## scatter_plot = pca_data_df.hvplot.scatter(x="PC1", y="PC2")
## Show plot
## scatter_plot
## Customizing labels and title
## Use the columns from the original scaled DataFrame as the index.
## Retrieve the weights of each feature for each principal component
## Display the DataFrame
