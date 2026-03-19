# Intelligent Data Quality Monitoring & Anomaly Detection Pipeline

##  Overview
This project implements an AI-powered data quality monitoring pipeline designed to validate datasets, detect anomalies, and improve overall data reliability. It simulates real-world data engineering workflows used in large-scale enterprise systems.

The pipeline integrates feature engineering, validation checks, and machine learning-based anomaly detection to proactively identify data issues.


##  Key Features
- Automated data validation (missing values, duplicates, schema checks)
- Feature engineering from timestamp data
- Machine learning-based anomaly detection (Isolation Forest)
- Real-time alert simulation for data quality issues
- Scalable and modular pipeline design


##  Tech Stack
- Python
- Pandas
- Scikit-learn (Isolation Forest)
- Matplotlib (Visualization)

##  Dataset
- Brazilian E-commerce Dataset (Olist) – Kaggle  
File used: `olist_orders_dataset.csv`


## Pipeline Workflow

1. **Data Ingestion**
   - Load raw dataset from CSV

2. **Data Validation**
   - Check missing values
   - Identify duplicates
   - Validate schema

3. **Feature Engineering**
   - Extracted time-based features:
     - Purchase Hour
     - Purchase Day
     - Purchase Month
     - Weekend Indicator

4. **Data Transformation**
   - Converted timestamps into numerical features
   - Handled missing values

5. **Anomaly Detection**
   - Applied Isolation Forest model
   - Identified abnormal data patterns

6. **Alert System**
   - Generated alerts for detected anomalies

## Results
- Successfully detected anomalies in transactional data
- Improved data reliability by identifying inconsistencies early
- Enabled proactive data quality monitoring

## Visualization
- Scatter plot of anomalies based on time-based features
- Clear separation of normal vs anomalous data points

## How to Run

1. Open Google Colab
2. Upload dataset: `olist_orders_dataset.csv`
3. Run the notebook step-by-step:
   - Data preprocessing
   - Feature engineering
   - Model training
   - Anomaly detection

## Key Highlights
- Built an end-to-end data quality pipeline
- Applied machine learning for anomaly detection
- Implemented feature engineering for real-world datasets
- Designed scalable data validation workflows

## Future Improvements
- Integrate Great Expectations for advanced validation
- Orchestrate pipeline using Apache Airflow
- Deploy pipeline on AWS (Lambda + S3)
- Add real-time monitoring dashboards

