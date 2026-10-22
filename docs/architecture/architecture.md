
# Architecture and Diagrams

The System Context, Use Case, and Component diagrams have been prepared. The table below summarizes the main elements represented in each diagram.


## Diagrams


| Diagram | Main elements | Diagram file |
|---|---|---|
| System Context Diagram | User; forecasting system; dataset/API or IoT source; external storage/service if used; inputs and outputs | ![System Context Diagram](https://github.com/Set001YT/air-quality-forecasting-iot-ml/blob/main/diagrams/exports/System%20Context%20Diagram.png) |
| Use Case Diagram | Load/select data; preprocess; train/evaluate model; request/view forecast; inspect metrics | ![Use Case Diagram](https://github.com/Set001YT/air-quality-forecasting-iot-ml/blob/main/diagrams/exports/Use%20Case%20Diagram.png) |
| Component Diagram (draft) | Ingestion; validation/preprocessing; storage; baseline/model training and inference; evaluation; presentation/API | ![Component Diagram (Draft)](https://github.com/Set001YT/air-quality-forecasting-iot-ml/blob/main/diagrams/exports/Component%20Diagram(draft).png) |


## Draft Component Flow

Data source → ingestion and validation → preprocessing/features → storage → baseline and ML forecasting → evaluation → forecast presentation/export.

## Architecture Overview

The proposed system includes data input, processing, storage, forecasting, evaluation, and presentation. Input data may come from a historical dataset or, if available, an API or IoT source.

The forecasting component is intended to support a baseline and a machine-learning model. Their performance will be evaluated under documented and comparable conditions.

The input layer is designed to allow future IoT integration. Physical sensor deployment and direct sensor integration are not assumed to be completed capabilities at this stage.

## Main Components

- **Data source:** historical air-quality dataset, API, or IoT source.
- **Ingestion and validation:** receives input records and checks their validity.
- **Preprocessing and features:** prepares data for forecasting.
- **Storage:** stores data or intermediate results where required by the implementation.
- **Baseline and ML forecasting:** produces forecasts using a baseline and a candidate machine-learning model.
- **Evaluation:** measures forecasting performance under comparable conditions.
- **Presentation/export:** makes forecast results available to the user.

## Scope and Limitations

The diagrams describe the proposed architecture. The exact forecasting target, forecast horizon, dataset, model, and final technology stack remain subject to confirmation based on data availability and project requirements.

Direct integration with physical IoT sensors depends on hardware availability.
