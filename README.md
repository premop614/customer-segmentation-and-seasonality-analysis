# Customer Segmentation and Seasonality Analysis

This project analyses customer behaviour using transactional e-commerce data and customer segmentation techniques. It was developed as the analytical part of my master’s thesis at Masaryk University.

The analysis combines RFM segmentation, K-means clustering, and seasonality analysis to identify customer groups, compare their purchasing behaviour, and examine how customer activity changes over time.

The goal of the project is to transform raw transactional data into practical insights that can support CRM activities, targeted marketing, and inventory planning.

## Objective

The main objective of this project is to analyse customer behaviour and identify meaningful customer segments. The analysis focuses on three key areas:

- identifying customer segments based on RFM characteristics  
- comparing behavioural differences across segments  
- analysing how customer activity changes over time, with an emphasis on seasonal patterns  

## Methodology

The analysis follows the CRISP-DM framework:

1. Business Understanding  
2. Data Understanding  
3. Data Preparation  
4. Modelling  
5. Evaluation  
6. Interpretation of results and business implications  

RFM variables were calculated at the customer level:

- **Recency** – number of days since the last purchase  
- **Frequency** – number of orders  
- **Monetary** – total customer spending  

The RFM variables were transformed into comparable scores using a quantile-based approach. K-means clustering was then applied to identify groups of customers with similar behaviour.

The number of clusters was selected using the elbow method and evaluated based on interpretability and clustering metrics.

Seasonality analysis was performed on aggregated time series data. Monthly trends, seasonal indices, and cluster-level seasonal behaviour were analysed, with attention to periods such as Back-to-School and Christmas.

## Key Findings

The analysis shows that customer value is unevenly distributed. A smaller group of customers generates a higher share of value, while most customers are concentrated in intermediate segments.

The RFM segmentation identified groups such as:

- Champions  
- Loyal Customers  
- Potential Loyalists  
- Promising Customers  
- At Risk Customers  
- Hibernating Customers  

The K-means clustering provided four broader behavioural groups:

- High-Value Customers  
- Repeat Customers  
- Inactive Customers  
- New Customers  

The seasonality analysis showed that customer activity differs across periods of the year. Some customer groups are more responsive during Back-to-School and Christmas periods, while others show more stable behaviour throughout the year.

## Visualisations

### RFM Segment Distribution

![Treemap of RFM Segments](treemap-rfm-segments.png)

### Elbow Method for K-means Clustering

![Elbow Method](elbow-method.png)

### Customer Clusters Visualised Using PCA

![PCA Clusters](pca-clusters.png)

### Seasonal Index of Orders

![Seasonal Index](seasonal-index.png)

### Orders by Cluster Over Time

![Orders by Cluster](orders-by-cluster-over-time.png)

### Seasonal Lift of Orders by Cluster

![Seasonal Lift Heatmap](seasonal-lift-heatmap.png)

## Business Implications

The results can support practical business decisions in several areas:

- targeted CRM and email marketing campaigns  
- reactivation of inactive customers  
- improved timing of seasonal promotions  
- better inventory planning before peak periods  
- customer value development through segment-specific communication  

## Skills Demonstrated

This project demonstrates practical skills in:

- data cleaning and preparation  
- exploratory data analysis  
- customer segmentation  
- RFM analysis  
- K-means clustering  
- seasonality analysis  
- data visualisation  
- business interpretation of analytical results  
- working with real transactional data  

## Repository Structure

```text
├── Master Thesis.pdf
├── README.md
├── analysis.ipynb
├── elbow-method.png
├── orders-by-cluster-over-time.png
├── pca-clusters.png
├── seasonal-index.png
├── seasonal-lift-heatmap.png
└── treemap-rfm-segments.png
```

## Tools and Technologies

- Python (Pandas, NumPy, Scikit-learn)  
- Jupyter Notebook  
- Excel  

## Note on Data

The original dataset is not publicly available because it contains company transactional data. The analysis notebook and thesis documentation are included to demonstrate the analytical workflow, methodology, and results.

The initial data exploration, quality assessment, and part of the data preparation were performed in Excel, while modelling and advanced analysis were implemented in Python.

## Author
Přemysl Opálka,
Master’s thesis project, Masaryk University
