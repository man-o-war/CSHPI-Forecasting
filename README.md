# CSHPI-Forecasting

## CSHPI Forecasting using VAR Model(as of now)

Forecasting S&P Case Shiller Housing Price Indices using various supply and demand factors using VAR(Vector Auto Regression) model. Data Collected from S&P Dow Jones and fred.saintlouis.edu

---

## Approach followed

1. Data collection
2. EDA
    * Preprocessing and timeseries resampling
    * Data joined
    * Visalizing
    * Stationarity Checks
3. Train Validation splitting
4. Model Training
5. Making Predictions
6. MSE metrics

---

## Key Decisions

1. Data resampled and considered in freq -> QS = Quarter Start
2. Ignore stationarity as some have it wrt others and some don't.
3. Train test splitting done manually to exert continuity when predicting.

---

## Key Observations

1. Covid and Recession of '08 causes Stationarity issues in even the stationary relations.
2. Predections are off because of above.
3. Possible required approach via LSTMs and averaging difference to deal with stationarity.
4. More co-dependent supply and demand factors are required, that cause CS_HPI to variate.
