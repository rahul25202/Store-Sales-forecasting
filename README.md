# Store Sales Forecasting

## Introduction 🌟

Cognizant of the dynamic retail landscape, this project is dedicated to the prediction of store sales for Corporación Favorita, a prominent Ecuadorian grocery retailer. Leveraging the power of time series forecasting, as well as machine learning and deep learning techniques, we endeavor to offer more precise sales predictions. This undertaking takes on the crucial task of enhancing inventory management while satisfying the ever-evolving needs of customers.

In  initial efforts,  XGBoost model achieved a score of 1.45784, reflecting a promising start for this time series project. While there's room for improvement, this performance serves as a solid foundation for further exploration.

This model reveals that key factors influencing sales include the product family, store number, and whether a product is being promoted or not.

## Key Objectives 🎯

primary goal is to develop a model that accurately predicts unit sales across thousands of products in Favorita stores. By improving forecasting accuracy,  aim is to reduce food waste due to overstocking and enhance customer satisfaction.

## Data Sources 📊

All data for this project was obtained from the [**Store Sales - Time Series Forecasting**](https://www.kaggle.com/competitions/store-sales-time-series-forecasting/data). The dataset includes various files with detailed information:

- **train.csv**: Training data with features such as store_nbr, family, onpromotion, and sales.
- **test.csv**: Test data for predicting future sales.
- **stores.csv**: Store metadata, including city, state, type, and cluster.
- **oil.csv**: Daily oil prices, an essential external factor.
- **holidays_events.csv**: Holidays and Events dataset, including information on transferred and bridge holidays.
and more ...
## Methodology 🚀

approach was to solve this problem includes the following key steps:
- Data preprocessing and cleaning.
- Feature engineering.
- Exploratory Data Analysis (EDA).
- Model development, including XGBoost and deep learning models.
- Model evaluation using the Root Mean Squared Error (RMSE) instead of RMSLE as the metric.

## Data Preprocessing 🛠️

cleaned the data, handled missing values, and performed one-hot encoding. Additionally, we merged external datasets such as oil prices and holiday events.

## Model Architecture 🏗️

model architecture is a fusion of two powerful techniques: XGBoost and deep learning models. Specifically,  employed the XGBoost model, a robust gradient-boosting algorithm, to capture essential patterns in the data efficiently. Additionally, we incorporate deep learning models to leverage their capacity to capture intricate temporal dependencies.

To ensure the best model performance,  implemented techniques like early stopping, which helps prevent overfitting by monitoring model performance during training. Furthermore, we utilize learning rate decay, which adjusts the learning rate over time to fine-tune model convergence and accuracy.

This combination of XGBoost and deep learning, along with strategic optimizations, empowers our model to provide accurate sales forecasts for the project.

## Training and Evaluation 📈

- **Optimization:** used the Adam optimizer with a learning rate of 0.001.
- **Loss Function:** Root Mean Squared Error (RMSE).
- **Epochs:** Training the XGBoost for 99 steps then stopped by early stopping.
- **Model Evaluation:** The final evaluation metric was Root Mean Squared Logarithmic Error (RMSLE).

## Conclusion 🎯

- Approach was resulted in accurate store sales predictions.
- Score: 1.45784 (lower is better).
- Key factors influencing sales include the product family, store number, and whether a product is being promoted or not
- This project has the potential to reduce food waste and enhance customer satisfaction for grocery stores.
