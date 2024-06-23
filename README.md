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
- **Histogram of Amount feature **:
  ![Histogram](https://github.com/amany-adel/Amazon-Sales-Data-Analytics-Task/blob/main/Visualization/Frequency%20of%20the%20Sales%20Amount.png)


- **Bar Plots of Ship state and Category  ![Bar Plot](https://github.com/amany-adel/Amazon-Sales-Data-Analytics-Task/blob/main/Visualization/Bar%20Plot%20of%20ship-state.png)


- **Top sales By city: !(https://github.com/amany-adel/Amazon-Sales-Data-Analytics-Task/blob/main/Visualization/Bar%20Plot%20of%20Total%20Sales%20by%20City.png)






# Example code for generating a histogram
plt.hist(data['Feature A'])
plt.title('Histogram of Feature A')
plt.xlabel('Value')
plt.ylabel('Frequency')
plt.savefig('histogram_a.png')
