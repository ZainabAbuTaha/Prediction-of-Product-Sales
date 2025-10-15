# Sales Prediction Project
 Author: Zainab Abu Taha



## Project overview 
The project aims to analyze 2023 sales data to understand seasonality and predict future performance. The primary issue addressed is the difficulty of forecasting actual sales in light of market changes, which impacts planning and production. This analysis helps companies build informed business models based on actual data.

This project is divided into 4 main parts: loading and inspecting the data, cleaning the data, and performing exploratory data analysis (EDA), feature insepection

## Business Problem
 - Retail companies often struggle to accurately forecast sales due to seasonal fluctuations and shifting market dynamics. This uncertainty can lead to overstocking, understocking, and missed revenue opportunities. The goal of this project is to build a predictive model that estimates item-level sales across different outlets, enabling better planning, resource allocation, and strategic decision-making.

## Data
 - Source: Public dataset simulating 2023 retail sales
 - Size: ~8,500 observations, 12 features
 - Features include product type, outlet characteristics, visibility, pricing, and historical sales

## Results
Here, I explored the data visually to find patterns, correlations, and insights.
- Visualized numerical features (e.g., histograms, boxplots).
- Analyzed categorical features using bar charts.
- Used a heatmap to explore feature correlations.

1️⃣ Histogram of item_Outlet_Sales (to visualize the distribution of a numerical feature):
<img width="790" height="390" alt="histogram" src="https://github.com/user-attachments/assets/af22e1ef-52bc-4393-9e63-cc52d161d1ca" />

2️⃣ Countplot of item_Type (to show the frequency of a categorical feature):
<img width="789" height="390" alt="plot1" src="https://github.com/user-attachments/assets/6e85c139-75ef-4c6b-adaf-96b0770aa1a5" />

## Predictive Modeling
### Linear Regression Coefficients
<img width="1353" height="659" alt="linear-reg" src="https://github.com/user-attachments/assets/f0e28a2a-10bc-43ce-8352-1f6bf2791ded" />
#### Top 3 Features:
Item_MRP (+979.46): Higher product prices result in higher sales.
Outlet_Type_Supermarket Type3 (+709.60): Type 3 supermarkets consistently perform better.
Outlet_Identifier_OUT027 (+709.60): This specific outlet has strong sales, likely due to location or size.

#### Negative Impact Features:
Grocery Stores and underperforming outlets decrease predicted sales.
Being in a small or low-performing outlet reduces sales potential.
Summary: Positive coefficients increase predicted sales, while negative coefficients decrease it. Linear Regression shows that product price and store type are strong drivers of sales.
### Random Forest Feature Importances
<img width="1357" height="676" alt="random-forest" src="https://github.com/user-attachments/assets/da55d8ff-40d0-424f-84a4-ef87323cebd4" />
#### Top 5 Features:
Item_MRP (0.5100): Higher-priced products sell more.
Outlet_Type_Grocery Store (0.2653): Outlet type heavily influences sales.
Item_Visibility (0.0455): Better shelf visibility improves product sales.
Outlet_Type_Supermarket Type3 (0.0454): These outlets consistently perform well.
Outlet_Identifier_OUT027 (0.0444): This top-performing outlet sells more than most others.
#### Summary: Random Forest confirms that price and store characteristics are the main drivers, while visibility and specific outlet performance also matter. The model captures non-linear patterns missed by Linear Regression.

## Methods
 - Cleaned and standardized missing values and inconsistent entries
 - Performed univariate and multivariate exploratory data analysis (EDA)
 - Identified and engineered relevant features for modeling
 - Built and evaluated multiple regression models using scikit-learn
 - Selected the best-performing model based on RMSE and R²

## Recommendations
 - Use the model to guide monthly inventory planning and promotional strategies
 - Prioritize high-variance product categories for deeper analysis
 - Integrate real-time sales data to retrain the model periodically
## Limitations & Next Steps
 - The dataset lacks time-series granularity, limiting seasonality analysis
 - Outlet-level promotions and competitor pricing were not included
 - Future work could incorporate external data (e.g., holidays, weather) and deploy the model via a dashboard

## Conclusion
This project showcases the full data preprocessing pipeline: from loading and inspecting raw data to cleaning and performing meaningful exploratory analysis. The insights gained lay the groundwork for further modeling or decision-making tasks.

## For Further Information
For questions or collaboration inquiries, please contact: zainab.k.abutaha@gmail.com
