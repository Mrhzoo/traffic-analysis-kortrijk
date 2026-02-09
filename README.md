# 🚦 Traffic Analysis Dashboard - Kortrijk

[![Python](https://img.shields.io/badge/Python-3.13-blue.svg)](https://www.python.org/)
[![Streamlit](https://img.shields.io/badge/Streamlit-1.52-red.svg)](https://streamlit.io/)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-1.8-orange.svg)](https://scikit-learn.org/)

An interactive traffic analysis and forecasting platform for Kortrijk using real-time Telraam sensor data, machine learning models, and weather integration. The system provides data-driven insights for urban planning and traffic management decisions.

## 🎯 Overview

This project analyzes traffic patterns across multiple transportation modes (cars, bicycles, pedestrians, heavy vehicles) in Kortrijk using:

- **Real-time data collection** from Telraam sensors
- **Weather integration** (temperature, precipitation, cloud cover, wind speed)
- **Machine learning forecasting** using Random Forest models
- **Interactive Streamlit dashboard** with 7 analysis tabs
- **Parking scenario simulation** to evaluate policy changes
- **Anomaly detection** using clustering algorithms

The dashboard processes 3,489+ hours of traffic data from two key streets near Howest Campus, providing  forecasts and comprehensive historical analysis.

## ✨ Key Features

- **Multi-modal traffic analysis**: Cars, bikes, pedestrians, heavy vehicles
- **Temporal patterns**: Hourly, daily, weekly trends with holiday effects
- **Weather correlation**: Impact of weather conditions on traffic volume
- **ML forecasting**: Random Forest models with 10 features and 5 prediction targets
- **Scenario analysis**: Compare open, closed, and paid parking impacts
- **Clustering & anomalies**: K-means clustering and Isolation Forest detection
- **Interactive visualizations**: Charts, heatmaps, and statistical summaries

## 🛠 Technology Stack

- **Python 3.13** - Core programming language
- **Streamlit 1.52** - Web dashboard framework
- **scikit-learn 1.8** - Machine learning models
- **pandas 2.3** - Data manipulation
- **Plotly 6.5 / Matplotlib 3.10** - Visualizations
- **PyArrow 22.0** - Efficient data storage (Parquet)
- **Prophet 1.2** - Time series forecasting

## 📊 Data Sources

- **Telraam Traffic Sensors**: Hourly traffic counts for Graaf Karel de Goedelaan and Sintmartenslatemlaan
- **Open-Meteo API**: Hourly weather data for Kortrijk
- **Calendar Events**: Belgian holidays and Flemish school vacation periods



## 🤖 Machine Learning Models

### Random Forest Architecture
- **Models**: 5 separate regressors (car, bike, pedestrian, heavy, total)
- **Features**: 10 variables (time, weather, calendar, location)
- **Training Data**: 3,489 hours of traffic data
- **Evaluation**: MAE and RMSE metrics

### Parking Scenarios
- **Open Parking**: Baseline (current conditions)
- **Closed Parking**: -50% cars, +40% bikes, +30% pedestrians
- **Paid Parking**: -20% cars, +20% bikes, +5% pedestrians

## 📱 Dashboard Tabs
<img width="1919" height="793" alt="image" src="https://github.com/user-attachments/assets/b8cad977-2edc-4b95-a079-19a4498535c4" />



1. **Overview**: KPIs, trends, and mode distribution
2. **Analysis**: Detailed patterns by mode, time, and location
3. **Weather Impact**: Temperature, precipitation, and conditions analysis
4. **ML Forecasts**:predictions with insights
5. **Parking Scenarios**: Policy impact comparisons
6. **Raod Block Scenarios**: Impact on a steet on a specifc choosen hours
7. **Clustering**: Traffic pattern groups and anomaly detection

## 🌐 Deployment

Deploy to Streamlit Cloud:
1. Push code to GitHub
2. Visit [share.streamlit.io](https://share.streamlit.io)
3. Connect repository: `Mrhzoo/traffic-analysis-kortrijk`
4. Set main file: `dashboard/app.py`
5. Deploy



## 👨‍💻 Author

**Hamzzah Kattan**

GitHub: (https://github.com/Mrhzoo)

---

*Built for urban mobility insights and data-driven traffic management*
