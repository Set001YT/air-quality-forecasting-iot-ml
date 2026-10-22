
# Verification and Evaluation Plan

The evaluation plan defines the proposed validation process and performance measures. The final target and applicable metrics will be confirmed after the dataset is selected and the forecasting task is specified.

## Testing and Evaluation

| Area | Method | Measure / Pass Condition |
|---|---|---|
| Input validation | Test valid records, missing fields, invalid types, and timestamp errors. | Invalid records are handled predictably, and errors are documented. |
| Preprocessing | Check missing-value handling, feature processing, and chronological order. | Valid features are produced without future information leakage. |
| Forecast quality | Compare the baseline and ML model on the same chronological hold-out period. | Report MAE/RMSE and R² where appropriate; select the model based on measured results. |
| Classification (if used) | Compare predicted and true AQI categories. | Report accuracy and, if useful, precision, recall, or F1. |
| Runtime | Measure inference time in the target environment. | Report observed latency; define a threshold after the environment is known. |
| Reproducibility | Repeat evaluation using recorded settings. | The same split and configuration reproduce results within the expected tolerance. |

## Baseline and Evaluation Conditions

- Use chronological train/validation/test splits for time-series data; do not mix future records into training.
- Compare models using the same target, forecast horizon, test period, and metrics.
- Document the data source, geographical coverage, date range, sampling interval, missing-data handling, and features.
- Do not promise accuracy before experiments; report measured results and limitations.
- Record the selected dataset, geographical coverage, observation period, sampling interval, available features, missing-data rate, and applicable usage terms before model training.
