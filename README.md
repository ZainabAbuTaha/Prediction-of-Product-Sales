# Sales Prediction Project

## Project overview 
The project aims to analyze 2023 sales data to understand seasonality and predict future performance. The primary issue addressed is the difficulty of forecasting actual sales in light of market changes, which impacts planning and production. This analysis helps companies build informed business models based on actual data.

This project is divided into 4 main parts: loading and inspecting the data, cleaning the data, and performing exploratory data analysis (EDA), feature insepection

## 🔹 Part 1: Load and Inspect Data
In this section, I loaded the dataset and performed a basic inspection to understand its structure.
- Loaded the dataset using pandas.
- Displayed the first few rows using df.head().
- Checked for data types, missing values, and general information using df.info() and df.describe().

## 🔹 Part 2: Clean Data
In this step, I prepared the data for analysis by handling missing or incorrect values.
- Handled missing values (e.g., dropping or filling).
- Converted data types where necessary.
- Removed duplicates and irrelevant columns if needed.

## 🔹 Part 3: Exploratory Data Analysis (EDA)
Here, I explored the data visually to find patterns, correlations, and insights.
- Visualized numerical features (e.g., histograms, boxplots).
- Analyzed categorical features using bar charts.
- Used a heatmap to explore feature correlations.

1️⃣ Histogram of item_Outlet_Sales (to visualize the distribution of a numerical feature):
<img width="790" height="390" alt="histogram" src="https://github.com/user-attachments/assets/af22e1ef-52bc-4393-9e63-cc52d161d1ca" />

2️⃣ Countplot of item_Type (to show the frequency of a categorical feature):
<img width="789" height="390" alt="plot1" src="https://github.com/user-attachments/assets/6e85c139-75ef-4c6b-adaf-96b0770aa1a5" />

## 🔹 Part 4: Feature Inspection
- Replaced placeholder values (e.g., 'Missing', 'NA') with proper nulls (np.nan)
- Inspected each feature individually using univariate visualizations
- Identified feature types: numeric, categorical (nominal/ordinal)
- Checked for missing values and calculated their percentages
- Evaluated cardinality and whether features were constant or quasi-constant
- Assessed whether each feature is known before the target is determined
- Determined if any feature should be excluded based on business logic
- Created multivariate plots to explore relationships with the target (Item_Outlet_Sales)
- Answered key inspection questions to decide which features are useful for prediction
- 
## Conclusion
This project showcases the full data preprocessing pipeline: from loading and inspecting raw data to cleaning and performing meaningful exploratory analysis. The insights gained lay the groundwork for further modeling or decision-making tasks.
