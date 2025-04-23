# CapstoneML-project



# 1. Overview 

Air pollution is a major global concern, affecting human health, climate, and ecosystems. Monitoring air quality is essential for understanding pollution levels, identifying key pollutants, and taking necessary actions to improve environmental conditions. However, with increasing urbanization and industrialization, air pollution levels continue to rise, posing serious health risks. This study aims to analyze air quality data to identify trends, detect anomalies, and understand the impact of various pollutants on environmental and human health.

# Dataset
Source
Dataworld :https://catalog.data.gov/dataset/air-quality
No:of Records 18025 rows and 12 columns

# Features
• Unique ID: A unique identifier for each data entry.

• Indicator ID: Represents different air quality indicators.

• Name: The name of the air quality indicator (e.g., “Ozone (O3)”, “Boiler Emissions- Total SO2 Emissions”).

• Measure: Specifies the type of measurement (e.g., “Mean”, “Number per km²”).

• Measure Info: Additional information about the measurement, such as units (e.g., “ppb”, “number”).

• Geo Type Name: The geographic level of the data (e.g., “UHF42”, “UHF34”).

• Geo Join ID: A numerical ID for joining geographic data.

• Geo Place Name: The name of the geographic area where data was collected.

• Time Period: The time period for which data was recorded (e.g., “Summer 2014”, “2015”).

• Start_Date: The exact start date of data collection.

• Data Value: The actual recorded air quality value. This is likely the target variable.

• Message: Contains additional notes, sometimes missing (NaN).

# Steps Used

1.Data Collection & Cleaning

2.Exploratory Data Analysis (EDA)

3.Feature Engineering

4.Feature Selection

5.Feature Scaling

6.Training and Testing

7.Model building

8.Model Evaluation

9.Hyperparameter tuning

10.Pipeline Implementation

11.Test with unseen data

# Libraries Used

1.pandas

2.numpy

3.matplotlib

4.seaborn

5.scikit-learn

6.joblib

# About the project

This project focuses on predicting air quality levels using machine learning techniques. The target variable in this analysis is Data Value, which represents the measured concentration of pollutants such as Nitrogen Dioxide (NO₂) and Ozone (O₃) in different areas of New York City.

I started the project with data preprocessing and cleaning, where I handled missing values, removed duplicates, and ensured the dataset was well-structured for analysis. After cleaning, I moved on to Exploratory Data Analysis (EDA) to understand the patterns, distributions, and relationships between different features and the target variable.

After EDA, I performed feature engineering, such as encoding categorical variables using one-hot encoding, and scaling numerical features. Then, I built and evaluated various regression models including Linear Regression, Decision Tree Regressor, Random Forest Regressor, Gradient Boosting, and others.

The Random Forest Regressor gave the best performance based on evaluation metrics like MAE, MSE, RMSE, and R² score. I further improved the model using hyperparameter tuning and wrapped all necessary steps into a machine learning pipeline for better scalability and reusability.

Finally, I tested the trained model using unseen data to simulate real-world performance and observed consistent predictions. I also saved the final model using joblib for future use.

This project was a great opportunity to strengthen my knowledge in machine learning workflows, model evaluation, and real-world data application. It also highlighted the importance of clean data, meaningful features, and proper tuning to build reliable and accurate predictive models.

# Results

•	After training and evaluating several regression models, Random Forest Regressor provided the best performance.

	•	The evaluation metrics for the best model were:
 
	•	Mean Absolute Error (MAE): ~1.75
 
	•	Mean Squared Error (MSE): ~7.10
 
	•	Root Mean Squared Error (RMSE): ~2.66

	•	R² Score: 0.91 – indicating that the model explains 91% of the variance in the target variable (Data Value).
 
	•	When tested with unseen data, the model returned consistent and reasonable predictions, suggesting strong generalization ability.
	•	These results show that the model can effectively predict air quality levels across different regions in New York City based on features like pollutant types and locations.
