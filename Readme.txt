# Transaction Clustering Analysis Project Archive

## Project Overview
This project aims to analyze transaction patterns and detect anomalies using clustering techniques. The dataset includes transaction data from 2013 to 2024, and various clustering algorithms were applied to discover hidden patterns and outliers.

## Dataset
The dataset contains yearly aggregated transaction amounts and other transaction-related attributes. The columns include:
- TRANS DATE: The date of the transaction.
- TRANS VAT DESC: Description of VAT applied.
- ORIGINAL GROSS AMT: The original transaction amount.
- ORIGINAL CUR: The original currency code.
- BILLING GROSS AMT: The billing transaction amount.
- BILLING CUR CODE: The billing currency code.
- TRANS TAX AMT: The transaction tax amount.
- MERCHANT NAME: The name of the merchant.
- CARD NUMBER: The card number used for the transaction.
- TRANS CAC CODE 1: Transaction code 1.
- TRANS CAC DESC 1: Description of transaction code 1.
- TRANS CAC CODE 2: Transaction code 2.
- TRANS CAC DESC 2: Description of transaction code 2.
- TRANS CAC CODE 3: Transaction code 3.
- Directorate: The directorate under which the transaction falls.
- Year: The year of the transaction.
- Month: The month of the transaction.
- Day: The day of the transaction.
- Cluster: The cluster label assigned to the transaction.
- KMeans_Labels: The cluster labels from KMeans clustering.

## Data Preprocessing
1. Converted categorical columns to string type for proper handling.
2. Standardized numerical features for clustering.
3. Applied clustering algorithms (KMeans and DBSCAN) to identify patterns and anomalies.

## Clustering Algorithms
### KMeans Clustering
KMeans clustering was applied to group transactions based on their attributes. The results revealed several distinct clusters with varying transaction amounts and patterns.

### DBSCAN Clustering
DBSCAN clustering was used to detect anomalies in the transaction data. This algorithm is effective in identifying outliers that do not conform to the general transaction patterns.

## Results
### Clustering Results Interpretation
- **Cluster 0**: Most prevalent, lower transaction amounts.
- **Cluster 1**: High-value transactions, potential anomalies.
- **Cluster 2**: Regular transactions, spread throughout the year.
- **Cluster 3**: Less frequent transactions, moderate amounts.
- **Cluster 4**: Occasional high-value transactions.

### Visualization
Various plots were generated to visualize the clustering results, including:
1. Distribution of transactions by month and year.
2. Top merchants by transaction count.
3. Transaction amounts by day of the month.
4. Box plots of transaction amounts across clusters.
5. Density plots for transaction amounts within clusters.

### Hypothesis Testing
A hypothesis was formulated and tested using statistical methods to validate the clustering results:
- Hypothesis: Transaction amounts in 2024 are significantly higher than in previous years.
- Result: The hypothesis was validated with a p-value < 0.05.

## Conclusion
The clustering analysis provided valuable insights into transaction patterns and identified potential anomalies. The results can be used to improve transaction monitoring and detect fraudulent activities.

## Future Work
- Further tuning of clustering algorithms.
- Exploring other clustering techniques like hierarchical clustering.
- Incorporating additional features for more comprehensive analysis.
- Implementing real-time anomaly detection systems.

Dataset link: https://www.cityobservatory.birmingham.gov.uk/@birmingham-city-council/purchase-card-transactions.