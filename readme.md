# Customer Segmentation Using Unsupervised Machine Learning

## Project Overview

This project applies **unsupervised machine learning** to identify customer segments for a German mail-order sales company using demographic data provided by Bertelsmann Arvato Analytics. The objective is to identify population groups that closely resemble the company's existing customers to support targeted marketing strategies and customer acquisition.

Using **Principal Component Analysis (PCA)** and **K-Means clustering**, the analysis identifies patterns in demographic characteristics and compares customer segments against the general population.

## Dataset

- **AZDIAS:** Demographic data representing the general German population.
- **CUSTOMERS:** Demographic information about existing customers.
- **Feature Attributes:** Metadata describing features and missing value codes.

*The original datasets are not included due to data-sharing restrictions.*

## Methodology

1. **Data Cleaning:** Assessed missing values, removed highly incomplete features, and developed a reusable `clean_data()` function to standardize preprocessing.
2. **Feature Engineering:** Transformed demographic variables and encoded categorical features.
3. **Feature Scaling:** Standardized numerical features to ensure comparability.
4. **PCA:** Reduced dimensionality while retaining important patterns in the data.
5. **K-Means Clustering:** Identified population segments and compared their representation among existing customers.

## Key Findings

| Cluster | General Population | Customers |
|---|---:|---:|
| Cluster 8 | 11.28% | 30.20% |
| Cluster 4 | 11.60% | 1.42% |

- **Cluster 8:** Overrepresented among customers, suggesting a promising segment for targeted marketing.
- **Cluster 4:** Underrepresented among customers, indicating weaker alignment with the existing customer base.

These findings demonstrate how clustering can identify potential target audiences and support data-driven marketing decisions. Additional campaign testing would be needed to confirm actual conversion rates.

## Technologies Used

**Python | Pandas | NumPy | Scikit-learn | Matplotlib | Seaborn | Jupyter Notebook**

## Conclusion

This project demonstrates how unsupervised machine learning can uncover meaningful customer segments within complex demographic data. By combining data preprocessing, dimensionality reduction, and clustering, the analysis provides insights that can help businesses better understand their customers and refine marketing strategies.

## Acknowledgments

Data provided by Bertelsmann Arvato Analytics through the Udacity Data Scientist program.