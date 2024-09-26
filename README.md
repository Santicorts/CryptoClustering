# Crypto Clustering Project

## Project Overview
This project aims to analyze and cluster various cryptocurrencies based on their market performance using machine learning techniques, particularly K-Means clustering. By reducing the dimensionality of the data using Principal Component Analysis (PCA), we compare clustering results from both original and PCA-transformed data to understand how feature reduction impacts clustering outcomes.

## Project Structure
- `CryptoClustering/`
  - `crypto_market_data.csv`: The dataset containing cryptocurrency market data
  - `Crypto_Clustering.ipynb`: Jupyter notebook containing the analysis and clustering
  - `README.md`: Project documentation file


## Dataset
The project utilizes the `crypto_market_data.csv` file, which contains the following features:
- `coin_id`: Identifier for the cryptocurrency.
- `price_change_percentage_24h`: Percentage change in price over the last 24 hours.
- `price_change_percentage_7d`: Percentage change in price over the last 7 days.
- `price_change_percentage_14d`: Percentage change in price over the last 14 days.
- `price_change_percentage_30d`: Percentage change in price over the last 30 days.
- `price_change_percentage_60d`: Percentage change in price over the last 60 days.

## Project Workflow
1. **Data Preprocessing**: 
   - Load the cryptocurrency data and handle any missing values.
   - Standardize the data to ensure features are on a comparable scale.

2. **K-Means Clustering**:
   - Perform K-Means clustering on the original standardized data.
   - Use the Elbow Method to identify the optimal number of clusters.

3. **Principal Component Analysis (PCA)**:
   - Apply PCA to reduce the dimensionality of the data to 3 principal components.
   - Perform K-Means clustering on the PCA-transformed data.
   - Use the Elbow Method to identify the optimal number of clusters for the PCA-transformed data.

4. **Visualization**:
   - Plot the Elbow curve for both the original and PCA-transformed data to compare the optimal number of clusters.
   - Create scatter plots to visualize the clusters formed by the original and PCA data.

## Results
- The optimal number of clusters was found to be similar for both the original and PCA-transformed data, suggesting that feature reduction did not significantly impact the clustering structure.
- Using PCA provided more interpretable and stable clusters, as it reduces noise and redundancy in the features.

## Conclusion
This project demonstrates how dimensionality reduction with PCA can simplify clustering tasks and improve the interpretability of results without losing significant information.

## How to Run the Code
1. Clone the repository or download the files.
2. Open the `Crypto_Clustering.ipynb` notebook in Jupyter Notebook or JupyterLab.
3. Run the cells sequentially to perform the analysis.

## Dependencies
- Python 3.6+
- pandas
- scikit-learn
- hvplot
- matplotlib
- Jupyter Notebook or JupyterLab

## Future Work
- Explore other clustering methods such as DBSCAN or Hierarchical Clustering.
- Include more features like trading volume or market capitalization to enhance the analysis.
- Develop a web-based application to visualize the clustering results dynamically.

## Author
Santiago Cortes


