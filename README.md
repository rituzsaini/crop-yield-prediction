# crop-yield-prediction

 1 Project Summary
This project aims to predict agricultural crop yield using machine learning techniques and compare the actual vs predicted yield across different crops, seasons, and regions. Accurate yield prediction helps in planning, food security, and supply chain optimization for both farmers and policymakers.

 2. Business Problem
Accurate crop yield estimation is critical for:

Optimizing resource allocation (fertilizers, irrigation, labor)

Reducing economic losses

Informing government procurement & food distribution

Improving food security and planning exports/imports

Manual estimation is time-consuming and prone to human error. This project leverages historical data and predictive modeling to automate the yield prediction process.

 3. Objectives
Build a predictive model to estimate crop yield.

Compare predicted yield with actual yield values.

Identify major factors influencing crop yield (e.g., rainfall, fertilizer usage).

Visualize the performance of the model with plots.

Derive insights to support agricultural planning and decision-making.

 4. Dataset Description
The dataset contains historical information on crops and yield, including:

Column Name	Description
Crop	Name of the crop (e.g., Rice, Wheat)
Crop_Year	Year of cultivation
Season	Season (e.g., Kharif, Rabi)
State	State/region of cultivation
Area	Total area under cultivation (hectares)
Production	Actual crop output (tonnes)
Annual_Rainfall	Rainfall received during cultivation (mm)
Fertilizer	Quantity of fertilizers used
Pesticide	Quantity of pesticides used
Yield	Actual yield (Production / Area)

 5. Methodology
Load and explore the dataset

Clean data (handle missing values, convert formats)

Feature engineering (calculate yield if missing, drop unimportant features)

Split data into training and testing sets

Train a machine learning model (e.g., Linear Regression, Decision Tree, Random Forest)

Evaluate the model

Plot actual vs predicted values

Draw insights and conclusions

 6. Data Preprocessing
Checked and handled missing/null values

Converted dates and text columns into categorical/numeric form

Normalized numeric columns like Area, Fertilizer, Rainfall

One-hot encoded categorical features like Crop, State, and Season

Split dataset into train and test sets (typically 80/20)

7. Model Building
A regression model (such as Linear Regression or Random Forest Regressor) was trained using features such as:

Area

Annual Rainfall

Fertilizer

Pesticide

Season

Crop

The target variable was Yield.

8. Evaluation Metrics
The model was evaluated using:

MAE (Mean Absolute Error): Measures average magnitude of errors.

MSE (Mean Squared Error): Penalizes large errors.

RMSE (Root Mean Squared Error): Standard deviation of residuals.

R² Score: Indicates how well predictions approximate actual data.

 9. Visualizations
Scatter Plot: Actual vs Predicted Yield

Line Plot: Predicted vs Actual trends over years

Feature Importance: Bar chart of top influencing factors

Error Distribution: Histogram of residuals

10. Key Insights
Rainfall and Fertilizer usage were strong predictors of yield.

Certain states consistently outperformed others in actual vs predicted yields.

The model showed high accuracy (R² > 0.85) on test data.

Pesticide had a weaker correlation than expected, suggesting misuse or overuse.

11. Tools and Technologies Used
Jupyter Notebook (Python)

Pandas, NumPy (Data wrangling)

Matplotlib, Seaborn (Visualization)

Scikit-learn (ML Modeling)

Regression Algorithms (Linear, Random Forest)

12. Future Improvements
Integrate real-time weather data via APIs

Include soil quality and NDVI (satellite vegetation index)

Deploy the model using Flask or Streamlit as a web app

Add geospatial analysis (GIS) for location-specific insights

13. Conclusion
The crop yield prediction model demonstrates strong potential in forecasting agricultural output using historical and environmental data. By visualizing the actual vs predicted values, the project bridges the gap between traditional farming knowledge and data-driven insights. This solution can be scaled to support farmers, agronomists, and policy-makers across the agriculture ecosystem.
