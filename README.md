# Mobipredict: Demand-Aware Fleet Optimizer
## Overview
Mobipredict is a machine learning-based project aimed at solving a critical problem faced by rental companies — how to optimally place vehicles at different locations based on predicted demand. Rental mobility startups often face challenges where some locations have too many vehicles sitting idle while others suffer from shortages, leading to customer dissatisfaction and lost revenue.

This project builds a demand forecasting system that predicts the number of bikes or cars needed at specific spots by analyzing multiple data sources including historical rental data, state-wise weather patterns, and regional holiday information. The goal is to enable fleet operators to make data-driven decisions for vehicle allocation, improving resource utilization and customer satisfaction.

## Problem Statement
Companies offering rented vehicles struggle with vehicle placement due to unpredictable demand patterns across locations and times. Incorrect vehicle distribution leads to:

- High demand but low availability in some areas.

- Surplus idle vehicles in other regions.

- Loss of business and poor customer experience.

Mobipredict addresses this by forecasting location-specific demand, helping companies allocate the right number of vehicles in the right places at the right time.

## Approach & Methodology
### Data Collection:
Due to the scarcity of local datasets, the project uses a dataset sourced from an international bike rental company operating in a similar domain. Additional features like weather conditions and holiday schedules were incorporated to improve prediction accuracy.

### Feature Engineering:
Extracted meaningful features from rental timestamps, weather data, and holiday calendars to capture temporal and environmental influences on demand.

### Modeling:
Employed advanced machine learning algorithms, including boosting techniques, to build a model that achieves approximately 89% accuracy in demand prediction.

### Automation & Pipeline:
Developed a modular CI/CD pipeline using GitHub Actions and MLflow to automate data preprocessing, model training, evaluation, and deployment. This ensures smooth lifecycle management and easy updates.

## Impact & Use Case
Mobipredict provides fleet operators, especially startups with actionable insights for smarter vehicle placement. By predicting demand more precisely:

- Customer wait times and dissatisfaction reduce.

- Fleet utilization improves by minimizing idle vehicles.

- Overall business efficiency and revenue increase.

## Future Work

- Integrate real-time data feeds for dynamic demand prediction.

- Expand dataset coverage to more regions and vehicle types.

- Build a user-friendly dashboard for fleet operators to visualize demand forecasts.


#### Share Demand Prediction

MLFLOW_TRACKING_URI=https://dagshub.com/alokchoudhary05/Bike-Demand-Prediction.mlflow \
MLFLOW_TRACKING_USERNAME=alokchoudhary05 \
MLFLOW_TRACKING_PASSWORD=05c8a8affc83399f07de856088bad3e295e42437 \
python script.py
