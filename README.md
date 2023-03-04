# Predictive Maintenance(PdM) using Bidirectional-LSTM with Optuna
## Dataset Description

Maintenance strategy can mainly be categorized into 3 strategies, Run-to-Failure (R2F), Preventive maintenance (PvM), and Predictive maintenance (PdM).

R2F: Only happens when equipment stops working.

PvM: Time-based maintenance/ Scheduled maintenance: periodically maintain usually based on time or process iteration.

PdM: Use predictive tools to determine when maintenance action needs to be taken.

The goal is to predict the Remaining Useful Life(RUL) of each type of machines.

All data comes from [C-MAPSS Aircraft Engine Simulator Data](https://data.nasa.gov/dataset/C-MAPSS-Aircraft-Engine-Simulator-Data/xaut-bemq) with noise features added.

## Data Preprocess
Mainly referenced the preprocess methods from [umbertogriffo](https://github.com/umbertogriffo/Predictive-Maintenance-using-LSTM) and [PHAM VAN VUNG](https://www.kaggle.com/code/phamvanvung/cmapss)

## Algorithms
- Stacked Multiple Bidirectional LSTM layers with Attention layer to build the prediction model.
- Utilized Optuna with TPESampler to **automatically optimize hyperparameters**, including Learning Rate, Number of Layers, Nodes, Dropout Rates,etc.

## Code
[Bi-LSTM Model with Optuna](https://github.com/Kev107034011/pdm-lstm-prediction/blob/main/Bi-LSTM%20Model%20with%20Optuna.ipynb)

