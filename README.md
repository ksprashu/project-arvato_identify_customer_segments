# Identify Customer Segments with Arvato Data

## Unsupervised Learning

### Objective

In this project, our Bertelsmann partners AZ Direct and Arvato Financial Solutions have provided two datasets one with demographic information about the people of Germany, and one with that same information for customers of a mail-order sales company. You’ll look at relationships between demographics features, organize the population into clusters, and see how prevalent customers are in each of the segments obtained.

### Installation

The project consists of a jupyter notebook which will run on a base installation of anaconda

### Project Details

Broadly, we go through the following steps

#### Data Analysis

1. Import and understand the general population data
2. Clean up columns and rows that have a large proportion of NaNs
3. Encode categorical columns into indicator variables
4. Feature engineer new columns from mixed type columns
5. Impute all remain NaNs based on the median
6. Create a clean-up function to perform above tasks on the testing dataset

#### Unsupervised Learning

1. Scale the features using StandardScaler
2. Run PCA to identify the optimal number of components
3. Build a PCA model with (selected) 125 components
4. Understand what features make up the top 3 Principal Components
5. Run KMeans to identify the optimal number of clusters
6. Build a KMeans model with (selected) 10 clusters
7. Predict cluster labels for the general population data

#### Customer Data

1. Import the customer data and put it through the cleaning function
2. Run the customer data through the Scaler, PCA model, and KMeans model already built
3. Add any missing /features that were not present in the customer data
4. Predict the clusters for the customer dataset

#### Analysis

1. Compare the proportion of population in each of the clusters for both population and customer dataset
2. Identify the over-represented and under-represented clusters of customer
3. Understand what are the main features that make up the likely customers and the unlikely customers

### Conclusion

From the analysis we see that the population that have a greater tendency of becoming customers typically live far away from city centers, have low movement habits, and live in sparsely populated residential neighborhoods. They also seem to have lived through the avantgarde movement, are more open minded, less price conscious, and earn good income.

The population that have least tendency of becoming customers are typically those that earn low income, aren't home owners, and put most of their money in savings or investments rather than spending. This population also tends to live in large families, in dense neighborhoods with many buildings. The individuals also have lived through a mainstream movement, and are composed of the elderly, or single individuals or new couples without children who move about a lot.
