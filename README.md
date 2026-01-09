# InDuStIaLfOrEcAsTiNgWELOVEIT
Se3 Forceatsting Datenanalyse


# data download link:
https://www.kaggle.com/datasets/csafrit2/steel-industry-energy-consumption

# docs to autoarima
https://alkaline-ml.com/pmdarima/modules/generated/pmdarima.arima.auto_arima.html

## Project Structure

- `src/main.ipynb`: The key file containing the main analysis and forecasting implementation.
- `src/brainstorming/`: Directory with experimental notebooks for different forecasting models (ARIMA, LSTM, Prophet).
- `data/`: Contains the dataset (steel_industry_data.csv).
- `scientific source/`: Stores non-web sources and scientific references.

## Installation

### Linux
```
cd src

python3 -m venv venv

source venv/bin/activate

pip install -r dependencies.txt
```

### Windows
```
cd src

python -m venv venv

venv\Scripts\activate

pip install -r dependencies.txt
```