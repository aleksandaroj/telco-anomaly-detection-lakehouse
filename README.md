# Telco Anomaly Detection Lakehouse

> Work in progress

## Overview
End-to-end lakehouse pipeline for telecom network anomaly detection built 
on Azure + Databricks.

## Stack
- Azure Data Lake Storage Gen2
- Databricks + Unity Catalog
- Delta Lake
- PySpark
- Autoloader
- Autoencoder (TensorFlow) — planned

## Architecture
Landing → Bronze → Silver → Gold → ML

Raw JSON data is ingested from ADLS Gen2 using Auto Loader, processed into Delta format, and prepared for neural network training.

## Status
- [x] Synthetic data generator
- [x] Autoloader & batch ingestion
- [ ] Bronze layer
- [ ] Silver transformations
- [ ] Gold feature engineering
- [ ] Autoencoder model
