# Geospatial Analysis & Forecasting Service Request Volumes by Neighbourhood
## Overview

This project involves geospatial analysis and forecasting of daily and monthly service request volumes by location. The ultimate goal is to optimize resource allocation and improve service delivery.

## Technologies Used

![Python](https://img.shields.io/badge/Python-%23000?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-%23150458?style=for-the-badge&logo=pandas&logoColor=white)
![Geopandas](https://img.shields.io/badge/Geopandas-%23004236?style=for-the-badge&logo=geopandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-%2300A3E0?style=for-the-badge&logo=matplotlib&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-%23F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-%23F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-%23013243?style=for-the-badge&logo=numpy&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-%231572B6?style=for-the-badge&logo=seaborn&logoColor=white)
![Shapely](https://img.shields.io/badge/Shapely-%233C7832?style=for-the-badge&logo=shapely&logoColor=white)
![Requests](https://img.shields.io/badge/Requests-%2334C6EB?style=for-the-badge&logo=requests&logoColor=white)
![Holidays](https://img.shields.io/badge/Holidays-%23F1C40F?style=for-the-badge&logo=python&logoColor=white)
![Pillow](https://img.shields.io/badge/Pillow-%23E5A24D?style=for-the-badge&logo=pillow&logoColor=white)
![WordCloud](https://img.shields.io/badge/WordCloud-%2330B5E3?style=for-the-badge&logo=python&logoColor=white)

## Features

- **Geospatial Analysis**: Visualize and analyze service request data across different locations.
- **Forecasting**: Predict future service request volumes on a daily and monthly basis.
- **Visualization**: Interactive maps and charts to help understand request patterns.

## Data Source

The data used in this project is sourced from the City of Edmonton Open Data Portal. Two datasets were used: **311 Requests** and **Neighbourhoods Data**. You can access the datasets and explore more information at [City of Edmonton Open Data Portal](https://data.edmonton.ca/).

## Trends Seen

### 1. Shift to Digital
<p align="center">
<img  width=45% src="https://github.com/hrmn-preet/City-of-Edmonton-311-Requests-Analysis-/blob/main/Images/2014-2024.png" alt="Request Volume 2014-2024">
<img width=45% src="https://github.com/hrmn-preet/City-of-Edmonton-311-Requests-Analysis-/blob/main/Images/2024.png" alt="Request Volume 2024">
<br>
<i>Downtown continues to be the area with the highest volume of requests, reflecting its high population density and activity levels.</i>
</p>

There has been a significant shift from phone requests to app-based requests over the last decade, indicating a growing preference for digital interaction.

### 2. Centralized Request Volume
<p align="center">
<img  width=80% src="https://github.com/hrmn-preet/City-of-Edmonton-311-Requests-Analysis-/blob/main/Images/neigh.png">
<br>
<i>Downtown continues to be the area with the highest volume of requests, reflecting its high population density and activity levels.</i>
</p>

### 3. Dominance of Roadway Maintenance
<p align="center">
<img width=80% src="https://github.com/hrmn-preet/City-of-Edmonton-311-Requests-Analysis-/blob/main/Images/business%20unit.png" alt="Business Unit Requests">
<br>
<i>The Roadways Maintenance and Operations unit is a major player in handling requests, managing nearly half of the total annual requests.</i>
</p>

## Prediction of Daily and Monthly Requests

<p align="center">
<img src="https://github.com/hrmn-preet/City-of-Edmonton-311-Requests-Analysis-/blob/main/Images/regression.png" alt="Regression Analysis of Requests">
</p>
<p align="center">
<img src="https://github.com/hrmn-preet/City-of-Edmonton-311-Requests-Analysis-/blob/main/Images/scatter.png" alt="Scatter Plot of Requests">
</p>
#### Model Performance Comparison (Daily)

| Metric                         | Linear Regression | Random Forest | XGBoost       |
|--------------------------------|--------------------|---------------|---------------|
| **Training MSE**                | 0.9529             | 0.1440        | 0.7273        |
| **Training R² Score**           | 0.6420             | 0.9459        | 0.7267        |
| **Test MSE**                    | 0.6292             | 0.6750        | 0.6114        |
| **Test R² Score**               | 0.6501             | 0.6246        | 0.6600        |


#### Model Performance Comparison (Monthly Forecasting)

| Metric                         | Linear Regression | Random Forest | XGBoost       |
|--------------------------------|--------------------|---------------|---------------|
| **Training MSE**                | 90.357             | 8.560         | 20.950        |
| **Training R² Score**           | 0.814              | 0.982         | 0.957         |
| **Test MSE**                    | 82.971             | 38.306        | 39.866        |
| **Test R² Score**               | 0.790              | 0.903         | 0.899         |
### Explanation:

- Regression Analysis: Three regression models were used for initial analysis - Linear Regression, Random Forest and XG Boost.
- The initial regression without any hyper tuning yielded the following results: 


- Zero error plot: This scatter plot illustrates the relationship between different variables in the service request data. It may be used to visualize patterns or correlations in the data, such as the volume of requests over time or by location.



## GeoPandas Usage

<p align="center">
<img width=80% src="https://github.com/hrmn-preet/City-of-Edmonton-311-Requests-Analysis-/blob/main/Images/geo.png" alt="GeoPandas Usage">
</p>


## Contributing

Contributions are welcome. Please submit issues or pull requests to enhance the project.
