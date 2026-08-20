# Customer Segmentation Using Machine Learning

## Project Overview

This project applies unsupervised machine learning to segment customers based on demographic characteristics, purchasing behavior, product preferences, and customer engagement.

The objective is to identify meaningful customer groups and generate targeted business strategies for each segment.

## Dataset

The project uses the Customer Personality Analysis dataset.

Original dataset:
- 2,240 customers
- 29 features

After data preprocessing:
- 2,237 customers
- 17 features used for clustering

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab

## Machine Learning Methodology

The project follows these steps:

1. Data loading
2. Data quality assessment
3. Data cleaning
4. Exploratory Data Analysis
5. Feature engineering
6. Feature scaling
7. K-Means clustering
8. Optimal cluster selection
9. Cluster validation
10. PCA visualization
11. Customer segment profiling
12. Business insight generation

## Feature Engineering

The following customer-level features were created:

- Total Spending
- Total Purchases
- Total Children
- Total Campaigns Accepted
- Total Purchase Channels
- Average Spending per Purchase
- Web Conversion Ratio
- Household Size
- Product Spending Shares
- Customer Tenure

## Cluster Selection

Multiple methods were used to determine an appropriate number of clusters:

- Elbow Method
- Silhouette Score
- Davies-Bouldin Score
- Calinski-Harabasz Score

Based on the combined evaluation and business interpretability, K = 3 was selected.

## Final Customer Segments

### 1. High-Value & Highly Engaged Customers

- 750 customers
- Highest income
- Highest spending
- Highest purchase frequency
- Strong campaign engagement
- Strong online conversion

Recommended strategies:
- VIP loyalty programs
- Premium offers
- Personalized recommendations
- Cross-selling and upselling

### 2. Regular / Moderate-Value Customers

- 905 customers
- Largest customer segment
- Moderate income
- Moderate spending
- Moderate purchase frequency

Recommended strategies:
- Loyalty rewards
- Personalized discounts
- Cross-selling
- Purchase-frequency incentives

### 3. Low-Value / Low-Engagement Customers

- 582 customers
- Lowest income
- Lowest spending
- Lowest purchase frequency
- Low campaign engagement
- Low web conversion despite relatively high website visits

Recommended strategies:
- Re-engagement campaigns
- Targeted discounts
- Personalized recommendations
- Website conversion-focused offers

## Key Business Insights

- High-value customers contribute substantially more spending and purchasing activity.
- Regular customers represent the largest segment and provide an opportunity for value growth.
- Low-value customers show a conversion opportunity because website visits are relatively high compared with web purchases.
- Product preferences vary significantly between customer segments.
- Segment-specific marketing strategies can be more effective than treating all customers identically.

## Results

The final model assigns every customer to one of three machine-learning-generated segments.

The final output is saved as:

`customer_segmentation_results.csv`

## Future Improvements

Potential future improvements include:

- Comparing K-Means with DBSCAN and hierarchical clustering
- Using automated hyperparameter optimization
- Building a customer lifetime value model
- Developing a recommendation system
- Deploying the segmentation model as a web application
- Creating an interactive Streamlit dashboard
- Adding real-time customer scoring