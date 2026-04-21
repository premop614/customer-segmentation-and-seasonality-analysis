# Customer Segmentation and Seasonality Analysis

This repository contains the analytical part of a master’s thesis focused on understanding customer behaviour using data-driven methods. The analysis is based on transactional data from an e-commerce environment and aims to identify patterns in customer purchasing behaviour.

The project combines RFM segmentation, K-means clustering, and seasonality analysis to provide a structured view of customer value and its development over time. The results are used to derive insights that can support marketing activities and inventory management.

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

RFM variables were calculated at the customer level, where Recency represents the time since the last purchase, Frequency the number of orders, and Monetary the total amount spent. These variables were transformed into comparable scores using a quantile-based approach.

K-means clustering was applied to identify groups of customers with similar behaviour. The optimal number of clusters was determined using the elbow method.

Seasonality analysis was performed on aggregated time series data. Monthly patterns and seasonal indices were used to identify fluctuations in customer activity across different periods of the year.

## Key Findings

The analysis shows that customer value is unevenly distributed, with a relatively small group of customers generating a higher share of revenue. Most customers are concentrated in intermediate segments, indicating potential for further development.

The clustering results confirm the presence of distinct behavioural groups, such as new, inactive, repeat, and higher-value customers. These segments differ not only in their overall value but also in their purchasing patterns over time.

Seasonal variation was observed in customer activity, particularly during specific periods such as Back-to-School and Christmas. Some customer segments show increased responsiveness during these periods, while others behave more consistently throughout the year.

## Repository Structure

├── README.md  
├── analysis.ipynb  
├── Master Thesis.pdf  

## Tools and Technologies

- Python (Pandas, NumPy, Scikit-learn)  
- Jupyter Notebook  
- Excel  

## Note

The data preparation and exploratory analysis were initially performed in Excel, while the modelling and advanced analysis were implemented in Python.# customer-segmentation-seasonality-analysis
This repository contains the analytical part of a master’s thesis focused on understanding customer behaviour using data-driven methods.

The project combines RFM segmentation, K-means clustering, and seasonality analysis to identify patterns in customer purchasing behaviour and provide actionable business insights.
