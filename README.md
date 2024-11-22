# Enhanced-Delivery-Model-
**1)Data Loading and Initial Exploration**
Objective: Load and explore the dataset to understand its structure and contents.
Actions:
Loaded the dataset using Pandas.
Performed an initial inspection (info() and describe()) to identify data types, missing values, and key statistics.
**2)Data Cleaning and Preprocessing**
Objective: Handle missing values, correct data types, and prepare the data for analysis.
Actions:
Updated data types for numerical columns (float64) and dates (datetime).
Dropped irrelevant columns (ID, Delivery_person_ID).
Replaced invalid NaN placeholders and filled missing values with appropriate strategies:
Used the median, mode, or random sampling based on the column's nature.
**3. Feature Engineering**
Objective: Extract meaningful features to enhance the predictive power of the model.
Actions:
Extracted temporal features from Order_Date (e.g., day, month, year, weekend/weekday).
Calculated preparation time from order and pick-up timestamps.
Computed distances between restaurant and delivery locations using geodesic calculations.
Encoded categorical variables using LabelEncoder.
**4. Exploratory Data Analysis (EDA)**
Objective: Identify patterns, relationships, and insights in the data.
Actions:
Visualized feature distributions and their relationships with the target variable.
Explored delivery time variations by Road_traffic_density, Weather_conditions, and other categorical features using count plots and box plots.
Examined correlations between numerical features using a heatmap.
**5. Data Splitting and Standardization**
Objective: Prepare the data for machine learning by splitting into training and testing sets.
Actions:
Split the dataset into features (X) and the target variable (y).
Standardized numerical features using StandardScaler to improve model performance.
**6. Model Selection and Hyperparameter Tuning**
Objective: Identify the best-performing machine learning model for predicting delivery times.
Actions:
Tried multiple models: Linear Regression, Decision Tree Regressor, Random Forest Regressor, and XGBoost Regressor.
Used GridSearchCV for hyperparameter tuning to optimize each model's performance.
Evaluated models using metrics like R², RMSE, and MAE.
**7. Final Model Training**
Objective: Train the best-performing model (XGBoost) with optimal hyperparameters.
Actions:
Trained the XGBoost model using the training data.
Evaluated the model's performance on the test set.
**8. Performance Evaluation**
Objective: Quantify the model's accuracy and error rates.
Metrics Used:
R² (R-squared): Explained variance of the target variable.
MAE (Mean Absolute Error): Average magnitude of errors.
RMSE (Root Mean Squared Error): Emphasizes larger errors.
Adjusted R²: Corrected R² for multiple predictors.
Explained Variance Score: Captures model's explanatory power.
**9. Advanced Visualizations**
Objective: Gain deeper insights and validate the model's predictions.
Actions:
Visualized feature importance to understand the key contributors to delivery times.
Analyzed residuals to check for biases and validate the model's fit.
Compared predicted values against actual delivery times.
![image](https://github.com/user-attachments/assets/1a4a13f2-fa16-48bb-98d4-38ab90f315b8)
![image](https://github.com/user-attachments/assets/2a0c823d-3b7a-4d69-a495-442c6cd0a1f3)
![image](https://github.com/user-attachments/assets/73a579a7-ea6f-4ba5-b208-f1eef52c36ee)
![image](https://github.com/user-attachments/assets/e915a662-9c69-4575-b302-a7d90168bbb0)


