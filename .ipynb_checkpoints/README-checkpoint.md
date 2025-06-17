## Retail Store Demand Forecasting

This repository contains a Jupyter Notebook (`Retail_Inventory_Forcaste_J.ipynb`) detailing a project focused on analyzing and forecasting product demand in retail stores. The project aims to leverage historical sales data to uncover patterns and develop predictive models for accurate future demand estimation, thereby optimizing inventory management and enhancing overall store operations.

-----



### Introduction

This project defines the main goals and objectives of analyzing product demand to improve retail operations. Accurate demand forecasting is critical in retail to prevent issues like overstocking (which incurs storage costs and potential waste) and stockouts (leading to lost sales and reduced customer satisfaction). By improving forecasting accuracy, retailers can streamline inventory, minimize these problems, enhance operational efficiency, and ultimately boost sales and customer satisfaction. The project specifically aims to develop an XGBoost-based predictive regression model for forecasting product demand using historical sales and operational data.

### Dataset Overview

The project utilizes a dataset from Kaggle.com: [Retail Store Inventory and Demand Forecasting](https://www.kaggle.com/datasets/atomicd/retail-store-inventory-and-demand-forecasting). The notebook reviews and utilizes this dataset for the forecasting task.

The dataset includes:

- **76000 observations** of product sales across various regions and time periods.
- Features include:
  - `Inventory Level`
  - `Price`, `Discount`, `Promotion`
  - `Competitor Pricing`
  - `Category` (e.g., Electronics, Furniture, Groceries)
  - `Region` (North, South, West)
  - `Weather Condition` (Rainy, Snowy, Sunny)
  - `Seasonality` (Spring, Summer, Winter)
  - `Epidemic` indicator

## 🧪 Models Used & Evaluation

### 1. **OLS Regression**
- **R²**: 0.442
- **RMSE**: 24.00  
- Limitations: linear assumptions, high sensitivity to outliers, heteroscedasticity.

### 2. **Random Forest Regressor**
- **R²**: 0.869
- **RMSE**: 17.00  
- Captures non-linearity, robust to outliers, good for feature importance analysis.

### 3. **XGBoost Regressor** ✅ *(Best Performing Model)*
- **R²**: 0.888
- **RMSE**: 15.73  
- Excellent handling of non-linearity and feature interactions, scalable to large datasets, robust to outliers and noise.


## 🛠️ Tools & Libraries

- Python 3.x
- pandas, numpy, matplotlib, seaborn
- statsmodels (for OLS)
- scikit-learn (for preprocessing and Random Forest)
- xgboost
  
### Conclusion

The project successfully analyzed and forecasted product demand in retail stores. The insights gained from uncovering patterns in past sales and the development of predictive models provide a foundation for data-driven decision-making. The accurate demand estimation facilitated by this project is intended to optimize inventory management, reduce instances of overstocking and stockouts, and enhance overall store operations, leading to improved sales and customer satisfaction.

### Contributions

The following individuals contributed to this project:

  * [Jagdish Mane](https://www.linkedin.com/in/jagdish-mane/)
  * [Sachin Shukla](https://www.linkedin.com/in/sks336/)
  * [Hanmant Kattimani](https://www.linkedin.com/in/hanmant-kattimani-b8323741/)

### References


- Zhenzuo Zhu. (2025). Retail Store Inventory and Demand Forecasting [Data set]. Kaggle. https://doi.org/10.34740/KAGGLE/DSV/11895299
- OpenAI. (2023). ChatGPT (Mar 14 version) [Large language model]. https://chat.openai.com/chat.
- Chen, T., & Guestrin, C. (n.d.). XGBoost Tutorials. XGBoost Documentation. https://xgboost.readthedocs.io/en/stable/tutorials/index.html
- Agresti, A., & Kateri, M. (2021). Foundations of statistics for data scientists: With R and Python. CRC Press. https://doi.org/10.1201/9781003144328
- Qi, Y. (2008). *Random Forests* [PDF]. Carnegie Mellon University. https://www.cs.cmu.edu/~qyj/papersA08/11-rfbook.pdf

---