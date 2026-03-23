# Customer Segmentation and Churn Analysis

## Project Overview
This project analyzes customer purchasing behavior, performs customer segmentation using RFM (Recency, Frequency, Monetary) analysis and clustering, and predicts customer churn using machine learning techniques. The objective is to extract meaningful insights that support business decision-making and customer retention strategies.

## Quick Highlights
- Analyzed 4,300+ customer records to uncover purchasing patterns  
- Performed RFM-based customer segmentation using K-Means clustering  
- Built a Random Forest model for churn prediction with ~84% accuracy  
- Identified high-value and at-risk customers for targeted strategies  
- Delivered actionable business insights to improve customer retention  

## Objectives
- Understand customer behavior through data analysis
- Segment customers based on purchasing patterns
- Identify high-value and at-risk customers
- Predict customer churn using a classification model

## Technologies Used
- Python  
- Pandas 
- Matplotlib, Seaborn  
- Scikit-learn  

## Project Workflow

### Data Preprocessing
- Cleaned the dataset by handling missing values and duplicates
- Removed invalid records such as negative quantities and zero prices
- Converted data types and created relevant features, including total revenue
- Standardized product descriptions for consistency 

### Exploratory Data Analysis
- Analyzed sales trends, top products, and customer purchasing behavior
- Visualized revenue distribution and purchase frequency
- Identified key contributing countries and products

### Customer Segmentation
- Applied RFM (Recency, Frequency, Monetary) analysis
- Used K-Means clustering to group customers into segments
- Identified high-value, regular, and at-risk customer groups

### Churn Prediction
- Defined churn based on customer inactivity and low purchase frequency
- Built a Random Forest classification model to predict churn
- Evaluated model performance using confusion matrix, precision, recall, and F1-score

## Key Insights
- A small percentage of customers contributes a significant portion of total revenue
- High-value customers can be effectively targeted for retention strategies
- RFM metrics provide strong indicators of customer behavior
- Customer activity patterns can help identify potential churn 

## Business Impact
- Enables identification of high-value and churn-risk customers
- Supports targeted marketing and retention strategies
- Improves decision-making through data-driven insights

## Model Performance and Limitations

The churn prediction model achieved an accuracy of approximately 84%, demonstrating strong overall performance.

### Performance Insights
- The model performs well in identifying non-churn customers
- Lower recall for churn customers indicates difficulty in detecting all at-risk users
- Class imbalance (fewer churn cases) affects the model’s ability to generalize for minority class

### Limitations
- Churn definition is based on inactivity and frequency thresholds
- Class imbalance leads to reduced performance in predicting churn customers
- The model may miss some potential churn cases
- External factors such as seasonality and customer intent are not considered

### Future Improvements
- Apply class balancing techniques (e.g., class weights, resampling)
- Improve recall for churn prediction
- Incorporate additional behavioral and temporal features
- Use more advanced models or ensemble techniques

## Project Structure
```
customer_segmentation_churn/
│
├── data/
│ ├── online_retail.csv
│ ├── cleaned_data.csv
│ └── rfm_data.csv
│
├── notebook/
│ ├── 01_Data_Understanding.ipynb
│ ├── 02_Exploratory_Data_Analysis.ipynb
│ ├── 03_customer_segmentation.ipynb
│ └── 04_retention_analysis.ipynb
│
├── .gitignore
└── README.md
```

## Dataset
The dataset used in this project is available in the data/ folder, including raw, cleaned, and RFM-transformed data used across different stages of the analysis.

## Conclusion
This project demonstrates how customer data can be used to generate actionable insights through analysis, segmentation, and churn prediction. It highlights the value of RFM-based segmentation in understanding customer behavior and supporting retention strategies.

While the model achieves strong overall accuracy, challenges such as class imbalance highlight opportunities for further improvement in churn prediction performance.
