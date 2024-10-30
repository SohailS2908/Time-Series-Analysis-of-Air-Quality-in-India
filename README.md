# Time-Series Analysis of Air Quality in India

This project is a comprehensive time-series analysis of air quality across multiple Indian cities, focusing on pollutants such as PM2.5, PM10, NOx, SO2, and Ozone. Leveraging machine learning models, the project aims to uncover seasonal trends, geographical patterns, correlations among pollutants, and predictive insights. The project was built using Python with data sourced from Kaggle's "Time-Series Air Quality Data of India (2010-2023)" dataset.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Data Processing](#data-processing)
- [Feature Engineering](#feature-engineering)
- [Modeling](#modeling)
- [Results](#results)
- [Conclusion and Future Scope](#conclusion-and-future-scope)
- [Installation](#installation)
- [Usage](#usage)
- [License](#license)

## Project Overview
The primary goal of this project is to analyze air quality trends across Indian states from 2010 to 2023. It examines pollutant data across seasons, evaluates temporal dependencies, and forecasts pollutant levels. Key objectives include:
- Identifying seasonal and geographical pollution patterns
- Visualizing pollutant trends and interactions
- Implementing predictive models to forecast air pollution levels

## Dataset
The project utilizes the Kaggle dataset “Time-Series Air Quality Data of India (2010-2023),” which includes pollutant data in CSV format for various Indian cities. Data processing utilizes libraries such as `os` and `glob` for automation and management.

### Source
- [Kaggle: Time-Series Air Quality Data of India](https://www.kaggle.com/datasets/abhisheksjha/time-series-air-quality-data-of-india-2010-2023)

## Data Processing
### Data Cleaning and Preprocessing
- Columns with over 60% missing values were dropped.
- Interpolation methods were used for remaining missing values.
- Outliers were removed for pollutants to ensure accurate representation of trends.

## Feature Engineering
To capture time-series dynamics, several features were engineered:
- **Date Components**: Extracted features such as day, month, and season.
- **Lagged Features**: Created lag features to capture historical pollutant levels.
- **Grouped Pollutants**: Aggregated pollutants into categories, such as Nitrogen Compounds and Particulate Matter, for efficient visualization and modeling.

## Modeling
### Model Selection
The models used include:
- Random Forest Regressor
- Gradient Boosting Regressor
- XGBoost Regressor

### Evaluation Metrics
Models were evaluated using Mean Absolute Error (MAE), Mean Squared Error (MSE), and R-squared.

## Results
Key insights include:
- Seasonal spikes in PM2.5 and NOx during winter months.
- High correlation among nitrogen compounds.
- Models successfully forecast pollutant peaks and show strong correlation patterns through heatmaps and seasonal analyses.

## Conclusion and Future Scope
The study highlights the use of machine learning for air quality prediction, with significant seasonal and annual trends identified. Future work can extend this analysis by:
- Integrating meteorological data (e.g., humidity, temperature)
- Implementing advanced models such as LSTM networks
- Enabling real-time monitoring through IoT sensors

## Installation
To run this project, ensure you have Python installed along with the necessary libraries:
```bash
pip install pandas numpy scikit-learn xgboost matplotlib seaborn

## Usage
1. Download the dataset from Kaggle.
2. Run the preprocessing script to clean and structure the data.
3. Use the modeling scripts to train and evaluate models on air quality data.
4. Visualize results through the provided plotting scripts.
