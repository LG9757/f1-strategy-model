# F1 Strategy Model

This is something I did several months ago but only just uploaded it to GitHub.
The project is a regression-based machine learning model which analyses practice data to predict lap times for each compound in the race, taking into account fuel load, part of the race, the driver, team, etc.
Then, using the predicted lap times, it should be able to determine an optimal strategy based on the total race time for each strategy.

## Technologies Used
- **Python** - Programming language
- **Pandas** - Data manipulation and analysis
- **XGBoost** - Gradient boosting machine learning algorithm
- **Scikit-learn** - Machine learning
- **NumPy** - Numerical computing
- **Matplotlib** - Data visualization

## Datasets
The model uses data from multiple sources:
- **Ergast API**: Historical F1 race data (lap times, results, drivers, constructors, circuits, pit stops)
- **OpenF1 API**: Tyre compound data and pit stop telemetry from 2023-2024 seasons
  
### Data Coverage
- **Seasons**: 2023-2024 (46 races)
- **Features**: Year, Circuit, Driver, Team, Lap Number, Lap Time, Tyre Compound, Stint, Tyre Life, Fuel Load
- **Compounds**: Soft, Medium, Hard (dry compounds only)

## Features

- Lap time prediction with fuel and tyre degradation modeling
- Circuit-compound normalization for accurate cross-track comparisons
- Pit stop strategy optimization
- Hyperparameter tuning with RandomizedSearchCV
- Comprehensive data preprocessing and outlier removal
- Feature importance analysis

## Running

### Prerequesits
Have Python 3.10+ installed. Then install the required packages:
pip install pandas numpy xgboost scikit-learn matplotlib seaborn requests

### Installation

1. Clone the repository
2. Navigate to the project directory
3. Open the Jupyter notebook
4. Run all cells


