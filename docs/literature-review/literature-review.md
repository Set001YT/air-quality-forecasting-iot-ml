
# Literature Review

The literature review draws on twelve sources published between 2021 and 2026. The studies cover IoT-based air-quality monitoring, forecasting methods, and integrated systems. The table summarizes their objectives, data, methods, findings, limitations, and relevance to the proposed project.

## Literature Review Table

| Source / Study | Research Objective | Dataset / Data | Methods | Findings and Limitations | Relevance to This Project |
|---|---|---|---|---|---|
| Moursi et al. (2021), *IoT-enabled monitoring and prediction on the edge* | IoT monitoring and edge forecasting | PM2.5; sensor and edge data | NARX hybrid, LSTM, XGBRF | Combines IoT data acquisition with edge/cloud prediction. Transferability depends on the setup. | Supports a modular IoT and forecasting architecture. |
| *Intelligent Forecasting of Air Quality and Pollution Prediction* (2022) | Compare machine-learning approaches | PM2.5 data | Linear Regression, Random Forest, KNN, Ridge, Lasso, XGBoost, AdaBoost | Results depend on the dataset and experimental setting. | Supports baseline-versus-model comparison. |
| Jabbar et al. (2022), *LoRaWAN-based outdoor monitoring* | Long-range outdoor monitoring | Pollutant and climate sensor measurements | Arduino, LoRaWAN, The Things Network (TTN), ThingSpeak, Virtuino | Primarily focuses on monitoring and sensor/network setup rather than forecasting. | Informs data acquisition and communication choices. |
| *Machine Learning Algorithms to Forecast Air Quality: A Survey* (2023) | Review air-quality forecasting research | 155 papers published between 2011 and 2021 | Survey and review | Maps forecasting approaches; coverage depends on the included literature. | Provides broad methodological context. |
| *AQI Prediction Using ML for Ahmedabad* (2023) | Predict AQI in Ahmedabad | CPCB/SAFAR data, 2015–January 2021 | SARIMA, SVM kernels, LSTM | RBF SVM was reported as the best among the tested methods; findings are city-specific. | Supports comparison of statistical, SVM, and recurrent methods. |
| *Prediction of AQI Using ML Techniques: Comparative Analysis* (2023) | Compare AQI prediction methods | City-specific AQI datasets | SVR, Random Forest Regression, CatBoost; SMOTE discussed | Results depend on the dataset and preprocessing. | Supports careful comparison of regression models. |
| *Attention Hybrid Deep Learning and Quantum-Inspired Optimization* (2024) | Improve AQI forecasting | Seoul data | ARIMA, attention CNN, LSTM, QPSO, XGBoost | Uses an advanced hybrid approach whose complexity may exceed the needs of the initial prototype. | Provides an advanced reference, not necessarily a default implementation choice. |
| *Supervised ML Approaches for Predicting Key Pollutants: Systematic Review* (2024) | Review supervised ML for pollutant prediction | Studies selected through PRISMA | Systematic review | Summarizes supervised ML research; conclusions depend on the review's search scope. | Supports the literature synthesis. |
| *Air Quality Forecasting Using ML: Comparative Analysis and Ensemble Strategies* (2025) | Compare models and ensembles | 9,357 hourly records; PM2.5, NOx, CO, and benzene | Multiple ML models, Bayesian optimization, stacking | The data are from 2004–2005 despite the 2025 publication date. | Informs evaluation design and highlights the importance of data age. |
| Yıldız and Sucuoglu (2025), *Real-Time IoT-Based Air Quality Forecasting* | Real-time low-cost IoT forecasting | Low-cost sensor and climate measurements | Raspberry Pi 5, preprocessing, cloud, GRU | Reports R² above 0.93 and latency below 130 ms in its setting; results are subject to site-specific and calibration limitations. | Provides a close end-to-end IoT and ML reference. |
| *Deep Learning-Based Forecasting for Urban India* (2026) | Urban forecasting using temporal neural models | Hourly Indian-city data, 2015–2020 | LSTM, CNN-LSTM, Transformer | Geographic and dataset-specific generalization requires assessment. | Informs consideration of deep-learning alternatives. |
| Yaseen (2026), *China Major Cities AQI Forecasting Using Integrative ML Models* | Forecast AQI across major Chinese cities | Beijing, Wuhan, and Xi’an | OMVMD–WLSSVM–GRM; LGBM/SATLDE | Uses a complex optimized hybrid approach. | Shows advanced alternatives without requiring their implementation in the initial prototype. |

## Critical Synthesis

The literature covers three connected but distinct areas:

1. **IoT data acquisition and monitoring.** These studies inform sensor integration, communication, and system architecture. Monitoring-only work should not be described as forecasting.
2. **Air-quality forecasting.** Methods range from regression and tree-based ensembles to recurrent neural networks and complex hybrid models.
3. **End-to-end systems.** These combine sensing, preprocessing, prediction, and presentation in a single workflow.

Reported results cannot be compared directly unless the dataset, forecast target, prediction horizon, test period, and evaluation metrics are aligned.

## Preliminary Research Gap and Project Direction

The reviewed literature includes existing systems that combine IoT and machine learning. Therefore, the project should not claim that this combination is unprecedented.

A practical direction is to develop a manageable and reproducible prototype with a clear baseline, one or more candidate ML models, consistent evaluation conditions, and an IoT-compatible data input design.

The project-specific contribution should be demonstrated through implementation, reproducible model comparison, and transparent reporting of limitations.
