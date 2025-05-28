# IEEE-Jordan-Modelthon-Used-Car-Price-Prediction

### The IEEE Jordan Modelthon - Used Car Price Prediction repository focuses on predicting the sale prices of used cars in Jordan using machine learning techniques. 
Here's a summary of the README file:

## Project Overview

- The goal is to predict optimal used car prices in Jordan based on historical listing data.
  
- The challenge involves handling Jordan-specific variables such as customs clearance, regional specifications, and Arabic labels.
  
- The final model is a hybrid CatBoost-LightGBM approach, achieving an RMSE of ~7,000 JOD on the public leaderboard.
  
## Dataset & Features

- train.csv: Contains 10K+ listings with 33 columns.
  
- test.csv: Same structure but without the target variable.
  
## Sample Features:

- Condition: New or Used.
  
- Regional_Specs: Middle East specifications.
  
- Car_Customs: Cleared or Not Cleared.

- Kilometers: Odometer reading.
  
- City: Amman, Zarqa, etc.
  
## Model Architecture

- Uses a hybrid regression approach:
  
- Final Prediction = 0.7 × CatBoost Prediction + 0.3 × LightGBM Prediction.
  
- Why This Blend?
  
- CatBoost: Handles categorical and Arabic features well.
  
- LightGBM: Fast with numeric and tabular data.

## Getting Started

- Requirements:
  
- pandas==1.5.3
  
- catboost==1.2
  
- lightgbm==3.3.5
  
- category_encoders==2.6.0
  
## - Installation:

git clone https://github.com/ishiita95-harvad/jordan-car-prices.git
cd jordan-car-prices
pip install -r requirements.txt
  



