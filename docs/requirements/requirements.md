
# Requirements Specification

The requirements below define the initial scope and acceptance criteria. The forecast target, horizon, and final dataset remain subject to confirmation based on data availability and supervisor feedback.

## Functional and Non-Functional Requirements

| ID | Requirement | Type / Priority | Acceptance Criterion |
|---|---|---|---|
| FR-01 | Accept air-quality records from a supported dataset/input source | Functional / Must | A sample dataset loads and fields are checked. |
| FR-02 | Preprocess input data before forecasting | Functional / Must | Missing values, types, timestamps, and features are handled by a documented pipeline. |
| FR-03 | Generate a forecast for a defined target and horizon | Functional / Must | Valid input produces a forecast; target and horizon are documented. |
| FR-04 | Provide a baseline forecast | Functional / Must | Baseline and ML results use the same test period. |
| FR-05 | Display or export forecast results | Functional / Must | User can inspect or retrieve forecast values and timestamps. |
| FR-06 | Calculate evaluation metrics | Functional / Must | MAE and RMSE are calculated; R² is used where suitable. |
| FR-07 | Support future IoT integration through a modular input interface | Functional / Should | Ingestion interface is documented and separated from model logic. |
| NFR-01 | Avoid temporal data leakage | Non-functional / Must | Time-series data use a chronological split; preprocessing fits training data only. |
| NFR-02 | Make results reproducible | Non-functional / Must | Dataset, preprocessing, split, settings, and metrics are documented. |
| NFR-03 | Keep the prototype modular | Non-functional / Should | Ingestion, preprocessing, forecasting, and presentation are separate components. |
| NFR-04 | Communicate limitations | Non-functional / Should | Documentation states coverage, horizon, limitations, and intended use. |
