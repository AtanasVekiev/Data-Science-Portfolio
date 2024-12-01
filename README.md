# Optimization of HVAC System Parameters Using Machine Learning

This project applies machine learning to optimize HVAC (Heating, Ventilation, and Air Conditioning) system parameters. By leveraging advanced algorithms and real-world data, the aim is to enhance operational efficiency and reduce energy consumption in HVAC systems.

## Introduction  
HVAC systems regulate indoor temperature, airflow, and air quality. While integral to modern buildings, they are often energy-intensive. This project addresses inefficiencies in HVAC operations by predicting optimal parameters for system functioning. Optimizing these systems can lead to significant energy savings, cost reduction, and environmental benefits.

## Dataset Overview  
The dataset contains time-series data, including features such as air temperature, humidity, and energy usage, collected from a real-world HVAC system. Key attributes include:  
- **Input Features:** Temperature, humidity, energy usage.  
- **Target Variable:** Supply air temperature.  

The dataset posed challenges like gaps, missing data, and complex feature interactions.

## Data Preprocessing and Feature Selection  
Applying sliding window sampling to capture temporal dependencies. Feature selection highlighted the most impactful variables for model predictions.

## Model Selection and Methodology  
Three models were employed:  
1. **Linear Regression**: Used as a baseline for comparison.  
2. **Random Forest**: Addressed non-linear relationships and provided feature importance insights.  
3. **XGBoost**: Optimized gradient boosting for improved accuracy.  

Evaluation metrics included Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE).

## Model Training and Optimization  
Data was split sequentially to maintain temporal integrity. Features were standardized before training. Hyperparameter tuning for Random Forest and XGBoost significantly improved predictions. Performance was evaluated using 15-minute and 30-minute sliding windows.

## Results and Conclusion  
The project achieved significant improvements in predicting HVAC parameters, with reductions in RMSE and MAE across tuning phases. These results demonstrate the potential of machine learning to optimize HVAC systems, leading to more efficient energy usage and cost savings.

## Dependencies
* pandas
* numpy
* scikit-learn
* xgboost
* matplotlib
* seaborn

## References
Relevant research papers, datasets, and documentation used in this project are cited within the notebook.
