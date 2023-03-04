# Predictive Maintenance(PdM) using Bidirectional-LSTM with Stratify Sampling
## Dataset Description

Maintenance strategy can mainly be categorized into 3 strategies, Run-to-Failure (R2F), Preventive maintenance (PvM), and Predictive maintenance (PdM).

R2F: Only happens when equipment stops working.<br>
PvM: Time-based maintenance/ Scheduled maintenance: periodically maintain usually based on time or process iteration.<br>
PdM: Use predictive tools to determine when maintenance action needs to be taken.

The goal is to predict the Remaining Useful Life(RUL) of each type of machines.

All data comes from [C-MAPSS Aircraft Engine Simulator Data](https://data.nasa.gov/dataset/C-MAPSS-Aircraft-Engine-Simulator-Data/xaut-bemq) with noise features added.

## Data Preprocess
Mainly referenced the preprocess methods from [umbertogriffo](https://github.com/umbertogriffo/Predictive-Maintenance-using-LSTM) and [PHAM VAN VUNG](https://www.kaggle.com/code/phamvanvung/cmapss)

## Algorithms
-Use stratify sampling to ensure the model can all machines pattern.<br> 
-Stacked Multiple Bidirectional LSTM layers to build the prediction model.




