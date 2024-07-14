# Prediction of Flight Delays

## TL;DR
This project aimed to predict flight delays using various machine learning techniques. It begins with exploratory data analysis (EDA) to understand the relationships between flight characteristics and delays. Feature engineering was applied to create new features, such as categorical representations of departure times and seasonal indicators. Three machine learning classification models—Logistic Regression, Random Forest, and XGBoost—were trained and evaluated.

## Conclusion
The overall performance of the models in predicting flight delays was promising. All models performed reasonably well, with XGBoost achieving the highest AUC score of 0.7372, indicating a superior ability to distinguish between delayed and non-delayed flights. Logistic Regression tended to predict delays (high sensitivity, low specificity), while Random Forest leaned towards predicting non-delays (low sensitivity, high specificity). The high recall and low specificity in Logistic Regression suggest potential overfitting. To improve performance, possible methods include implementing resampling techniques like SMOTE, adding more contextual features (such as weather data), or using a grid search with a higher range of parameters.

## Source Data
[Flight Delay and Cancellation Dataset (2019-2023)](https://www.kaggle.com/datasets/patrickzel/flight-delay-and-cancellation-dataset-2019-2023?resource=download)

## Project Structure
1. [Reading Dataset](#reading-dataset)
2. [Exploratory Analysis](#exploratory-analysis)
   1. [General Overview Analysis](#general-overview-analysis)
   2. [Delay Analysis](#delay-analysis)
3. [Feature Engineering](#feature-engineering)
   1. [Features Setup](#features-setup)
   2. [Features Filtering](#features-filtering)
   3. [Features Correlation Analysis](#features-correlation-analysis)
4. [Model Training and Evaluation](#model-training-and-evaluation)
   1. [Logistic Regression](#logistic-regression)
   2. [Random Forest](#random-forest)
   3. [XGBoost](#xgboost)
5. [Conclusion and Future Work](#conclusion-and-future-work)
