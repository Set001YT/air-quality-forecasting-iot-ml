
# Technology Comparison

The options below are based on the reviewed literature. Not every option was compared directly in the cited studies.

## Technology Decision Table

| Decision | Alternatives | Advantages | Trade-offs | Preliminary Direction |
|---|---|---|---|---|
| Data acquisition | Physical sensors; historical/public datasets; hybrid approach; AirData.kz Open Air Quality Dataset for Kazakhstan; Beijing Multi-Site Air Quality Dataset (UCI) | Sensors support live data; datasets support repeatable experiments. | Hardware adds cost and calibration requirements; datasets may not represent live local conditions. | Start with historical data and an IoT-compatible input interface; add sensors only if available. Evaluate AirData.kz as the primary candidate for Kazakhstan-focused forecasting and use the UCI Beijing dataset as a separate methodological alternative if needed. |
| Data transfer | Wi-Fi; LoRaWAN; dataset/API ingestion | Wi-Fi is straightforward; LoRaWAN supports long-range, low-power networks; APIs and datasets support reproducible experiments. | Wi-Fi requires network access; LoRaWAN requires compatible hardware and a gateway; API availability varies. | Use dataset/API ingestion initially and keep the interface modular. |
| Forecasting | Regression/SARIMA; Random Forest/XGBoost; LSTM/GRU | A baseline supports comparison; tree models suit tabular features; recurrent models capture temporal patterns. | Performance depends on data and forecast horizon; deep learning requires more tuning and data. | Compare a baseline with at least one tree-based model; add GRU/LSTM only if justified. |
| Storage | SQLite; PostgreSQL; cloud IoT/data platform | SQLite is simple for local use; PostgreSQL supports a structured backend; cloud platforms simplify some services. | SQLite has concurrency limits; PostgreSQL requires setup; cloud platforms add configuration and dependencies. | Use SQLite for a minimal local prototype or PostgreSQL for a separate backend; decide after the architecture is finalized. |
| Processing/deployment | Server/cloud; edge; hybrid | Server-side processing is simpler to develop; edge processing can reduce latency; hybrid approaches distribute work. | Edge devices have resource constraints; cloud processing needs connectivity; hybrid approaches add complexity. | Start with server-side forecasting and modular components. |

## Technology Inventory Across the Reviewed Papers

| Category | Technologies / Methods Identified |
|---|---|
| Acquisition and sensing | Physical IoT sensors; PM2.5 and other pollutant measurements; temperature/humidity; historical datasets |
| Communication / IoT platforms | LoRaWAN; Wi-Fi; Arduino Uno; Raspberry Pi; The Things Network (TTN); ThingSpeak; Virtuino |
| Statistical / baseline | Linear Regression; Ridge; Lasso; ARIMA; SARIMA |
| Tree-based and ensemble ML | Random Forest; XGBoost; AdaBoost; CatBoost; LightGBM; stacking |
| Other classical ML | KNN; SVM/SVR; Bayesian Ridge; Elastic Net; Decision Tree |
| Deep learning | LSTM; GRU; CNN-LSTM; CNN-GRU; Transformer; Attention CNN |
| Hybrid / optimization | NARX hybrids; ARIMA + attention CNN + QPSO-LSTM + XGBoost; OMVMD–WLSSVM–GRM with LGBM/SATLDE |
| Evaluation metrics | MAE; MSE; RMSE; R²; classification accuracy; inference latency |

## Selection Principle

The inventory lists methods identified in the reviewed papers. It does not mean that every method will be implemented. The final selection should be small enough to evaluate under the same conditions.
