# Scalable-Ride-Demand-Prediction-using-a-Distributed-ETL-Pipeline.

📌 Project Overview

This project builds a scalable ETL pipeline for processing NYC taxi ride data and predicting hourly ride demand.

The objective is to transform raw ride data into structured, analytics-ready datasets and develop machine learning models for demand forecasting.

This project follows the CRISP-DM methodology and aligns with distributed data engineering principles.
<hr>
🏗️ Project Architecture

Raw Data (Parquet)
→ Data Cleaning & Transformation
→ Feature Engineering
→ Aggregation (Hourly Ride Count)
→ Structured Storage
→ Machine Learning Models

📊 Dataset

NYC Taxi Ride Dataset (Parquet format)

Features include:

Pickup & dropoff timestamps

Trip distance

Passenger count

Fare amount

Location IDs

⚙️ ETL Pipeline

The ETL process includes:

Data ingestion from raw Parquet files

Cleaning missing & invalid values

Feature extraction (hour, day of week, weekend)

Aggregation of hourly ride counts

Structured data storage for modeling

🤖 Modeling

We implemented:

Linear Regression

Random Forest Regressor

📈 Best RMSE: ~"    "rides (Random Forest)

Tree-based models captured nonlinear demand patterns more effectively.

🚀 Future Improvements

Integrate Apache Spark for distributed scalability

Add weather & holiday features

Deploy prediction model via API

Build visualization dashboard

📂 Repository Structure
├── 01_Data_Cleaning.ipynb
├── 02_ETL_and_Data_Storage.ipynb
├── 03_Modeling_and_Evaluation.ipynb
├── data/
└── README.md
👥 Team

Harshavardhan J – ETL Pipeline & Modeling

Cuthbeth – Data Storage, CRISP-DM & Documentation
