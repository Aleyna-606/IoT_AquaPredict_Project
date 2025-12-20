# IoT_AquaPredict_Project
IoT and Applied Data Science Course Project: Smart Agriculture - Irrigation Needs Estimation
# IoT AquaPredict: Smart Agriculture Irrigation Prediction

This project focuses on optimizing agricultural water usage by predicting irrigation requirements through IoT sensor data analysis.

## Project Overview
The system analyzes **Soil Moisture (MOI)**, **Temperature**, and **Humidity** to determine whether a crop requires irrigation. This is a **Binary Classification** problem designed to support smart farming decisions.

## Dataset Summary
The dataset contains **16,411 records** with the following key features:
* **MOI (Moisture Index):** Soil moisture content, ranging from 1 to 100.
* **temp (Temperature):** Ambient temperature in Celsius, ranging from 13°C to 46°C.
* **humidity:** Relative humidity percentage, ranging from 15% to 91%.
* **result:** Target variable where **1** indicates irrigation is needed and **0** indicates it is not.

## Technical Infrastructure & Objectives
* **Success Metric:** Our target is to achieve a minimum of **90% Accuracy** for the final predictive model.
* **Baseline Models:** Initial modeling will involve **Logistic Regression** and **Decision Tree** algorithms.
* **Latency Constraints:** The model must provide predictions with a latency of less than **5 minutes**.
* **Future Scalability:** Documented **AWS account setup prerequisites** for future cloud deployment.

## AWS Deployment Plan
As per the project guidelines, this project will be deployed on an **AWS EC2 (Free Tier)** instance.
* **Server:** Ubuntu Server 22.04 LTS on a `t2.micro` instance.
* **Setup:** A virtual card will be used for account registration to ensure secure billing management.
* **Security:** Security Groups will be configured for SSH (Port 22) and Dashboard access (Port 8501).
* **Goal:** The final model API or Streamlit dashboard will be accessible via the EC2 public IP.

## Getting Started
1. Clone the repository: `git clone https://github.com/Aleyna-606/IoT_AquaPredict_Project.git`
2. Run the ingestion notebook: `notebooks/01_data_ingestion.ipynb`.