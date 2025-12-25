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

## Live Deployment Details
The predictive model is successfully deployed and running on an AWS cloud environment.
* **Instance Type:** AWS EC2 t3.micro (Free Tier Eligible)
* **Operating System:** Ubuntu 24.04.3 LTS
* **Public IPv4 Address:** `16.16.207.161`
* **Security:** Access is restricted via RSA Key Pair and monitored with AWS Billing Alerts.

## Getting Started
1. Clone the repository: `git clone https://github.com/Aleyna-606/IoT_AquaPredict_Project.git`
2. Run the ingestion notebook: `notebooks/01_data_ingestion.ipynb`.