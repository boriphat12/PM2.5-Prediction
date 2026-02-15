# 🌫️ PM2.5 Air Quality Forecasting: Bangkok

![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
![XGBoost](https://img.shields.io/badge/Model-XGBoost-orange)
![Optuna](https://img.shields.io/badge/Tuning-Optuna-lightgrey)
![Status](https://img.shields.io/badge/Status-Completed-green)

A Machine Learning project to **forecast PM2.5 concentrations 1 hour in advance** for Bangkok, Thailand. The model is designed to simulate a real-world warning system scenario, strictly avoiding data leakage by using only historical data (Lag features) and temporal information.

## 📌 Project Overview

Air pollution (PM2.5) is a critical health issue in Bangkok. This project aims to build a robust forecasting model that can predict future air quality levels without relying on concurrent weather data (which is unknown in a real-time forecasting context).

**Key Performance:**
- **R² Score:** 0.9600 (Excellent Fit)
- **RMSE:** 16.29 µg/m³
- **MAE:** ~10.51 µg/m³

## 📂 Repository Structure

```bash
├── main.py                 # Script to fetch data from OpenWeatherMap & Open-Meteo APIs
├── pm25_prediction.ipynb   # Main notebook: EDA, Cleaning, Feature Engineering, Modeling (XGBoost)
├── .env                    # API Keys (Not included in repo)
└── README.md               # Project documentation