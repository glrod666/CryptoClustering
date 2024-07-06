# CryptoClustering

Normalize the Data**:
    - Use `StandardScaler` from `scikit-learn` to normalize the data from the CSV file.
    - Create a DataFrame with the scaled data and set the "coin_id" index from the original DataFrame as the index for the new DataFrame
    ![Sample Image](Screenshot01.png)


## Finding the Best Value for k

1. **Using the Original Scaled Data**:
    - Use the elbow method to find the best value for k:
      - Create a list with the number of k values from 1 to 11.
      - Compute the inertia for each k value and store it.
      - Plot a line chart to visually identify the optimal k value.
     
![Sample Image](Elbowcurvescreenshot.png)
    

       ## Clustering Cryptocurrencies
         ### Original Scaled Data

1. **Cluster the Data**:
    - Initialize the K-means model with the best value for k.
    - Fit the model and predict clusters.
    - Added the predicted clusters to the original DataFrame.


