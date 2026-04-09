# Delhi Air Quality Forecasting and Pollution Risk Early Warning System

## Project overview
This project builds an end-to-end data science pipeline to forecast next-day PM2.5 levels in Delhi using air-quality and meteorological data from 2025.

The project combines:
- air-quality data collection
- weather data collection
- data cleaning and merging
- next-day PM2.5 forecasting
- model comparison
- pollution risk categorisation
- research-oriented interpretation

## Objective
The main objective is to predict next-day PM2.5 concentration and translate it into a practical pollution risk category.

## Data sources
- Open-Meteo Air Quality API
- NASA POWER Daily API

## Final dataset
The final modeling dataset contains:
- daily air-quality variables
- daily weather variables
- next-day PM2.5 target
- risk category labels

## Models tested
- Baseline persistence model
- Linear Regression
- Random Forest

## Main result
The baseline persistence model performed best, outperforming the tested machine learning models.

## Outputs created
- processed modeling dataset
- model comparison table
- risk summary table
- PM2.5 time-series plot
- correlation matrix
- final metrics summary

## Project status
Notebook pipeline completed successfully.

## Methodology summary
1. Collected hourly air-quality data for Delhi from Open-Meteo Air Quality API for 2025.
2. Collected daily weather data for Delhi from NASA POWER for 2025.
3. Aggregated hourly air-quality data to daily averages.
4. Merged daily pollutant and meteorological datasets by date.
5. Created next-day PM2.5 as the prediction target.
6. Built baseline, Linear Regression, and Random Forest models.
7. Evaluated models using MAE, RMSE, and R2.
8. Created pollution-risk categories from next-day PM2.5.

## Key results
- Final modeling dataset size: 364 rows and 12 columns
- Best model: Baseline persistence
- Baseline MAE: 15.52478250915751
- Baseline RMSE: 22.963507026633046
- Baseline R2: 0.6284562026479149
- Best non-baseline model: Linear Regression with lag features

## Project files
- `data/raw/delhi_air_quality_hourly_2025.csv`
- `data/raw/delhi_weather_daily_2025.csv`
- `data/processed/delhi_pm25_model_data_2025.csv`
- `data/processed/delhi_pm25_model_data_with_risk_2025.csv`
- `outputs/model_comparison_2025.csv`
- `outputs/risk_summary_2025.csv`
- `outputs/delhi_daily_pm25_2025.png`
- `outputs/correlation_matrix_2025.csv`
- `outputs/final_metrics_summary_2025.csv`
- `notebooks/delhi_air_quality_forecasting_2025.ipynb`