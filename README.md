# HIV-model
Spatiotemporal Bayesian forecasting model of HIV-infection spread in Ukraine (2014-2025) with statistical analysis

# HIV Spread Model in Ukraine (2014-2025)

A comprehensive spatiotemporal analysis and forecasting model for HIV/AIDS spread across Ukrainian regions using Bayesian methods.

## Overview

This project presents an end-to-end solution for analyzing and forecasting HIV/AIDS morbidity patterns across all regions of Ukraine. The work combines data engineering, statistical analysis, and machine learning technique to provide insights into disease spread dynamics.

### Current Application

The trained model is currently being used by the **Ministry of Health of Ukraine** to forecast HIV morbidity over time for each region of Ukraine. This deployment supports:

- **Public Health Planning**: Evidence-based resource allocation across regions
- **Early Warning System**: Identification of regions at risk of increased HIV incidence
- **Policy Making**: Data-driven decisions for prevention and intervention programs
- **Regional Targeting**: Prioritization of high-risk areas for health campaigns

The model provides actionable insights that directly contribute to national HIV/AIDS prevention and control strategies.

## Project Objectives

- Extract and standardize HIV/AIDS case data from monthly regional reports (2014-2025)
- Identify temporal trends and spatial clusters in disease spread
- Build a predictive model for regional HIV morbidity forecasting
- Provide open-source model and dataset for public health research


## Project Workflow

### Part 1: Data Preparation and Cleaning

**Objective**: Transform unstructured monthly HIV/AIDS reports into a structured, analysis-ready dataset.

**Process**:
- Collected monthly regional reports covering all Ukrainian regions (2014-2025)
- Implemented automated data extraction using OpenAI API
- Standardized data formats and resolved inconsistencies
- Validated data quality and completeness
- Published cleaned dataset to Kaggle for public access 

**Output**: Structured time-series dataset with regional HIV/AIDS case counts

**Dataset**: [Available on Kaggle](#) *(https://www.kaggle.com/datasets/kostyaprisych/hiv-aids-data-for-ukraine)*

### Part 2: Statistical Analysis (`analysis.ipynb`)

**Objective**: Understand disease spread patterns and identify key trends.

**Methods**:
- **Time Series Analysis**: Examined temporal trends in HIV incidence across regions
- **Spatial Analysis**: Identified geographic clusters and hotspots
- **Pattern Recognition**: Detected short-term and long-term trends
- **Correlation Studies**: Analyzed inter-regional relationships

**Key Findings**:
- Identified high-prevalence regions and temporal patterns
- Discovered spatial clustering of cases
- Revealed trends in disease progression over the 10-year period

### Part 3: Model Building and Evaluation (`bayesian_model.ipynb`)

**Objective**: Develop a predictive model for regional HIV morbidity forecasting.

**Model Architecture**: Bayesian Spatiotemporal Model

**Features**:
- Incorporates both spatial (regional) and temporal (time-based) dependencies
- Captures uncertainty through Bayesian inference
- Allows for region-specific predictions

**Training Configuration**:
- Training set: 70% of data (2014-2021)
- Test set: 30% of data (2022-2025)
- Cross-validation applied for robustness

**Performance Metrics**:
| Metric | Value |
|--------|-------|
| Accuracy | 77% |
| MAPE | 29% |
| R² Score | 0.78 |
