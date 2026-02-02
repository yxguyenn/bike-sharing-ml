# Bike Sharing Demand Prediction

## Overview
This project builds and evaluates machine learning models to predict hourly bike rental demand using weather and temporal features from the Bike Sharing dataset (UCI or Kaggle).

You can use either:
- **UCI Bike Sharing Dataset** (hour.csv / day.csv), or
- **Kaggle Bike Sharing Demand** (train.csv / test.csv)

This repo is set up to work with a single CSV placed at: `data/bike_sharing.csv`.

## Quickstart

1) **Create a virtual environment (optional)**
```bash
python -m venv .venv
source .venv/bin/activate  # mac/linux
# .venv\Scripts\activate  # windows
```

2) **Install dependencies**
```bash
pip install -r requirements.txt
```

3) **Add your data**
Place a CSV file at:
- `data/bike_sharing.csv`

Supported formats:
- UCI hourly/day: columns like `cnt`, `season`, `yr`, `mnth`, `hr`, `weekday`, `weathersit`, `temp`, `atemp`, `hum`, `windspeed`
- Kaggle: columns like `datetime`, `count`, `season`, `weather`, `temp`, `atemp`, `humidity`, `windspeed`

4) **Run the notebook**
Open `bike_sharing_ml.ipynb` in Jupyter/VSCode and run all cells.

## What the notebook does
- Loads and inspects the data
- Handles basic cleaning (drops obvious ID columns, removes leakage)
- Creates time features (if datetime exists)
- Builds preprocessing pipelines (numeric scaling + categorical one-hot encoding)
- Trains and compares:
  - Linear Regression
  - Random Forest Regressor
  - Gradient Boosting Regressor
- Evaluates using RMSE and R² on a train/validation split

## Tools
Python, NumPy, Pandas, scikit-learn, Jupyter Notebook

## Notes
- This project intentionally focuses on **clean, internship-friendly ML practice**:
  data prep → modeling → evaluation → conclusions.
- If you want, you can extend it with time-series splits, cross-validation, or hyperparameter tuning.
