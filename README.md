# EDA Report

## 1. Introduction
The purpose of this analysis is to explore the dataset to understand key characteristics and relationships within the data. Specifically, we aim to identify trends and potential outliers.

## 2. Data Overview
### Data Description
The dataset used in this analysis contains 128975 records and 24 features. The key features include Amount, Status, Caregory.

### Data Cleaning
The following data cleaning steps were performed:
- Missing values were imputed using the median for numerical features and Filling it with NONE or UNKNOWN for categorical features.
- Searching for wrong data types
- Data types were corrected for Date column.
- Outliers deletion.

## 3. Summary Statistics
### Descriptive Statistics
| Feature | Mean     | Min  | Max  | Std Dev  |
|---------|------    |------|------|--------- |
| Amount  |648.561465|  0   | 5584 |281.211687|




## 4. Data Visualizations
### Univariate Analysis
- **Histogram of Feature A**: ![Histogram](histogram_a.png)

### Bivariate Analysis
- **Scatter Plot of Feature A vs. Feature B**: ![Scatter Plot](scatter_ab.png)

### Multivariate Analysis
- **Pair Plot of Features A, B, and C**: ![Pair Plot](pairplot.png)

## 5. Key Findings
### Patterns and Trends
- Feature A shows a normal distribution with a mean of 10.5.

### Correlations and Relationships
- There is a strong positive correlation between Feature A and Feature B.

### Anomalies and Outliers
- Several outliers were identified in Feature C, which may warrant further investigation.

## 6. Conclusion
The EDA revealed several key insights, including a strong correlation between Feature A and Feature B. Further analysis could involve investigating the causes of outliers in Feature C.

## 7. Appendix
### Code
```python
import pandas as pd
import matplotlib.pyplot as plt

# Example code for generating a histogram
plt.hist(data['Feature A'])
plt.title('Histogram of Feature A')
plt.xlabel('Value')
plt.ylabel('Frequency')
plt.savefig('histogram_a.png')
