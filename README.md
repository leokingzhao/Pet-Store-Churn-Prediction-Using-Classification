# Pet-Store-Churn-Prediction-Using-Classification
This project builds an end-to-end pipeline for customer segmentation and churn prediction. Using RFM analysis, K-means clustering, and classification models with SHAP interpretation, it identifies high-risk customers and supports targeted retention strategies.

## Business Context
Customer churn is a critical issue that directly impacts revenue and growth. By segmenting customers and predicting churn, the business can proactively implement personalized offers, loyalty programs, and retention campaigns to reduce churn and improve overall performance.

## Approach

### 1. RFM Analysis
- **Recency**: Days since the last purchase  
- **Frequency**: Number of transactions  
- **Monetary**: Total spending  
- Customers are scored and categorized into segments using percentile-based bins.

### 2. K-means Clustering
- Combine RFM scores with transaction features.  
- Apply the Elbow Method to determine the optimal number of clusters.  
- Group customers into meaningful loyalty levels.  
- Compare results with RFM-based segmentation using metrics such as silhouette score.

### 3. Churn Prediction
- Define churn as no purchase within a 90-day period.  
- Build classification models (Logistic Regression, Random Forest, Gradient Boosting).  
- Evaluate with precision, recall, F1, and ROC-AUC.  
- Logistic Regression is selected for its balance of interpretability and performance.  
- Use **SHAP analysis** to interpret model predictions and identify key churn drivers.

## Key Insights
- Recency and profit margin strongly influence churn likelihood.  
- Segment-based modeling allows more accurate prediction and targeted strategies.  
- The pipeline provides both descriptive (segmentation) and predictive (classification) insights.

## Repository Structure
