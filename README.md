# Delhi-AQI-Predictive-Model
# Delhi PM2.5 Predictive Dashboard

![Dashboard Demo](Delhi%20aqi%20project.gif)

## 📋 Project Overview
Urban air quality is a critical public health challenge. This project moves beyond basic historical analysis by using machine learning to predict PM2.5 pollution spikes across six major monitoring stations in Delhi. The goal is to provide a functional, data-driven tool that can help shift urban planning from reactive to proactive.

## 🏗️ Technical Implementation
I built this end-to-end pipeline covering data processing, machine learning, and interactive visualization:
* **Data Engineering:** Built a robust pipeline (Pandas) to ingest, clean, chronologically sort, and impute missing values for over 50,000 hours of atmospheric data.
* **Predictive Modeling:** Trained a **Random Forest Regressor** (Scikit-Learn) using 13 atmospheric features (NO2, Ozone, Wind Speed, etc.) to forecast PM2.5 levels. 
* **Behavioral Segmentation:** Applied **K-Means Clustering** to group neighborhoods by their specific pollution profiles, demonstrating the need for localized interventions.
* **Interactive UI:** Designed a dark-themed, responsive frontend (Dash, Plotly, Bootstrap) featuring geospatial heatmaps, dynamic feature exploration, and real-time model evaluation metrics.

## 💡 Key Takeaways
1. **Geospatial Hotspots:** The interactive map clearly isolates persistent concentration zones, showing exactly where mitigation efforts should be prioritized.
2. **Leading Indicators:** Feature importance tracking reveals that specific atmospheric markers act as early-warning signals for severe PM2.5 spikes.
3. **Hyper-Local Volatility:** Time-series tracking proves that pollution variance between stations is high, meaning city-wide blanket policies are less effective than neighborhood-specific strategies.

## 🚀 How to Run Locally
1. Clone this repository.
2. Install dependencies: `pip install dash plotly scikit-learn pandas dash-bootstrap-components`
3. Run the application: `python app.py` (or execute the Jupyter notebook).
4. Navigate to the local host link provided in your terminal.
