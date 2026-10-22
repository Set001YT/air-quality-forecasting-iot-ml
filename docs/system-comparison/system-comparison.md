
# Existing System Comparison

The table compares four systems described in the reviewed papers. "Not specified" means that the source reviewed for this comparison did not provide enough information to confirm the feature.

## Comparison Table

| Criterion | A. Moursi et al. (2021) | B. Jabbar et al. (2022) | C. Yildız & Sucuoglu (2025) | D. Urban India Temporal DL (2026) |
|---|---|---|---|---|
| Primary purpose | Monitoring and forecasting | Outdoor monitoring / long-range transfer | Real-time IoT monitoring and forecasting | Air-quality forecasting |
| Physical IoT sensing | Yes | Yes | Yes | Not specified |
| Forecasting | Yes | Not central | Yes | Yes |
| Edge processing | Edge/cloud | Not specified | Raspberry Pi 5 edge layer | Not specified |
| Cloud/platform | Edge/cloud | TTN and visualization platforms | Cloud transfer, storage, and visualization | Not specified |
| ML methods | NARX hybrid, LSTM, XGBRF | Not central | GRU and other compared models | LSTM, CNN-LSTM, Transformer |
| Visualization | System-dependent | ThingSpeak/Virtuino | Cloud visualization | Not specified |
| Evaluation | Prediction evaluation | Measurement/monitoring validation | Forecast metrics and latency | Forecast model comparison |

## Comparative Interpretation

- **Moursi et al. (2021):** Integrates IoT data with edge/cloud prediction and serves as an architectural reference.
- **Jabbar et al. (2022):** Demonstrates sensor acquisition and LoRaWAN communication, but is primarily a monitoring system.
- **Yıldız and Sucuoglu (2025):** Is the closest end-to-end reference in this comparison. Its results are tied to its hardware, site, and evaluation conditions.
- **Urban India temporal DL (2026):** Informs temporal-model comparison, but the available summary does not establish a physical IoT sensing pipeline.

## Implications for the Proposed Project

The project should combine the capabilities required by its scope: data input, preprocessing, storage, forecasting, presentation, and measurable evaluation.

The project should not claim that this combination is unprecedented. Its contribution should be demonstrated through implementation, reproducible model comparison, and clear reporting of limitations.
