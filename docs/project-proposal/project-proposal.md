
# Project Proposal

## Project Title and Team

**Project title:** Development of an Air Quality Forecasting System Based on IoT and Machine Learning

**Team members:** Iskander Ismagulov and Asset Iglikov, SE-2427, BSc Software Engineering, Astana IT University.

**Supervisor:** Marzhan Turarova (Turarova Marzhan Kabdykalievna).

## Problem Statement

Air quality changes over time and may affect public health and everyday decisions. Monitoring systems describe current or past conditions, while users may also benefit from short-term forecasts. This project addresses the engineering problem of developing a system that receives air-quality-related data, processes it, applies a machine-learning model, and presents forecast results in an understandable form.

## Relevance

Air pollution is a relevant environmental issue for urban areas, including Astana. IoT can support environmental data acquisition and transfer, while machine learning can identify patterns in historical observations and produce short-term forecasts. The project will investigate how these elements can be combined in a practical, testable prototype.

## Target Users

- Residents interested in current and near-future air-quality conditions.
- Users interested in environmental monitoring and pollution trends.
- Researchers or students exploring IoT-based environmental data and forecasting.

## Aim

To design and develop a prototype system for forecasting air quality using IoT-compatible data acquisition and machine-learning methods, and to evaluate its performance using defined metrics.

## Objectives

- Review recent research on IoT-based air-quality monitoring and ML forecasting.
- Compare existing systems and alternative technologies relevant to the project.
- Define functional and non-functional requirements with acceptance criteria.
- Design the system architecture and required diagrams.
- Select and prepare a historical air-quality dataset and define an IoT-compatible ingestion interface.
- Establish a baseline and compare it with at least one ML model.
- Develop a prototype for data processing, forecasting, and presenting results.
- Test the prototype and evaluate forecast quality and relevant system performance.
- Document implementation decisions, limitations, and evaluation results.

## Proposed Solution

The planned prototype consists of a data input layer, preprocessing, data storage, a forecasting component, and a results presentation layer. Initial model development and evaluation will use a suitable historical dataset. The input layer should allow later integration of physical IoT measurements if hardware is available; physical sensor deployment is not assumed as a completed capability.

## Expected Outcomes

- Documented system design and prototype.
- Prepared dataset and reproducible preprocessing workflow.
- Baseline and ML forecasting model evaluated under comparable conditions.
- Results view showing forecast outputs and relevant air-quality information.
- Test/evaluation report stating metrics, limitations, and conditions.

## Scope and Limitations

The scope includes requirements analysis, system design, data preparation, model comparison, prototype implementation, and evaluation.

The exact forecast target (pollutant concentration or AQI), forecast horizon, dataset, model, and final technology stack must be fixed after checking data availability and requirements. Direct sensor connection depends on hardware availability. The prototype is not intended to replace certified measurement stations or provide medical advice.

Two candidate datasets are being considered:

- **AirData.kz Open Air Quality Dataset for Kazakhstan:** relevant to the project's intended geographical context.
- **Beijing Multi-Site Air Quality Dataset (UCI Machine Learning Repository):** a separate multi-station time-series dataset for methodological comparison.

The final dataset selection will depend on data coverage, completeness, available variables, and suitability for the chosen forecasting target.

## Project Management and Quality Assurance

Work should be tracked through a shared GitHub or GitLab repository and YouTrack. Tasks should have an owner, expected outcome, acceptance criteria, and deadline. Documentation, diagrams, and code should be committed progressively, with identifiable contributions from both students. Significant changes should be reviewed before merging.
