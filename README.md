Travel & Transportation Analytics using Big Data

Capstone Project – MBA (General) | University of Hyderabad
Author: Likhitha Sree Donda
Duration: Nov 2025

🧭 Project Overview

This project demonstrates how Big Data Analytics can optimize operations in the Travel & Transportation industry — focusing on ride-sharing and airline sectors.
The project consists of 5 analytical use cases, each addressing real-world business challenges such as dynamic pricing, route optimization, fraud detection, and ride demand forecasting.

All models were developed and visualized using Databricks (PySpark + Python) and Power BI / Plotly Dash.

⚙️ Tech Stack
Category	Tools / Technologies
Languages	Python, SQL, PySpark
Libraries	Pandas, Matplotlib, Seaborn, Scikit-learn, MLlib
Platform	Databricks Community / Azure
Visualization	Plotly Dash, Power BI
Storage	Delta Lake / Parquet
Version Control	GitHub
Documentation	Markdown + PPT Presentation
🏗️ Data Pipeline Architecture
Data Sources (APIs, CSV, IoT)
          │
          ▼
Ingestion Layer (PySpark / Databricks)
          │
          ▼
Storage Layer (Raw, Processed, Curated in Delta/S3)
          │
          ▼
Processing Layer (ETL, Feature Engineering)
          │
          ▼
Modeling Layer (MLlib / scikit-learn)
          │
          ▼
Visualization Layer (Dash / Power BI)


Each use case leverages the same unified data pipeline for ingestion, cleaning, analysis, modeling, and dashboard generation.

📁 Project Structure
📦 Travel-Transportation-Analytics
│
├── data/
│   ├── travel_transportation_dataset.csv
│   ├── processed/
│   └── raw/
│
├── notebooks/
│   ├── case1_smart_pricing.ipynb
│   ├── case2_route_optimization.ipynb
│   ├── case3_fast_matching.ipynb
│   ├── case4_fraud_detection.ipynb
│   └── case5_ride_prediction.ipynb
│
├── dashboards/
│   ├── case1_dashboard.png
│   ├── case2_dashboard.png
│   ├── case3_dashboard.png
│   ├── case4_dashboard.png
│   └── case5_dashboard.png
│
├── models/
│   ├── smart_pricing_model.pkl
│   ├── fraud_detection_rf_model.pkl
│   └── ride_forecast_model.pkl
│
├── scripts/
│   ├── data_pipeline.py
│   ├── preprocess.py
│   ├── utils.py
│
├── README.md
└── requirements.txt

🚀 Setup Instructions
🧩 1. Clone Repository
git clone https://github.com/<your-username>/Travel-Transportation-Analytics.git
cd Travel-Transportation-Analytics

⚙️ 2. Create Virtual Environment
python -m venv venv
source venv/bin/activate   # (Mac/Linux)
venv\Scripts\activate      # (Windows)

📦 3. Install Dependencies
pip install -r requirements.txt

🧠 4. Run the Pipeline
python scripts/data_pipeline.py

💻 5. Launch Dashboards (optional)

Use Databricks notebooks or Power BI to visualize dashboard .png outputs.

🧠 Use Case Summaries
1️⃣ Smart Pricing – Dynamic Pricing Model

Goal:
Predict dynamic fare prices based on demand, weather, traffic, and distance.

Model: Linear Regression (Fare Prediction)
Inputs: distance, demand_level, traffic_level, weather, base_fare
Outputs: predicted_fare

KPIs:

Fare Accuracy (%)

Demand–Fare Correlation

Surge Pricing Factor

Visuals:

Average Fare by Demand

Weather Impact Chart

Fare Correlation Heatmap

2️⃣ Best Routes – Route Optimization Model

Goal:
Identify efficient routes minimizing travel time and fuel cost.

Model: Regression / Optimization Model
Inputs: distance, traffic_level, route_type, fuel_cost
Outputs: optimal route suggestion

KPIs:

Average Speed (km/h)

Travel Time Variability

Fuel Efficiency Index

Visuals:

Speed vs Distance

Route Time Variability Chart

Fuel Cost by Traffic

3️⃣ Fast Matching – Driver–Rider Matching Model

Goal:
Improve matching efficiency between drivers and riders using proximity and traffic analytics.

Model: Classification / Logistic Regression
Inputs: driver_distance, demand_level, driver_rating, traffic_level
Outputs: match_efficiency_score

KPIs:

Match Success Rate (%)

Average Wait Time (min)

Rating Correlation

Visuals:

Distance vs Efficiency Scatter

Efficiency Heatmap by Traffic & Demand

Rating Correlation Plot

4️⃣ Safety Check – Fraud Detection Model

Goal:
Detect fraudulent ride transactions based on behavior, fare, and ratings.

Model: RandomForestClassifier
Inputs: total_fare, driver_rating, payment_method, traffic_level, demand_level
Outputs: fraud_probability (0 = Genuine, 1 = Fraud)

KPIs:

Accuracy & Recall (%)

Fraud Rate (%)

False Positive Rate

Visuals:

Fraud by Payment & Traffic

Rating Distribution (Fraud vs Genuine)

Feature Importance Chart

5️⃣ Ride Prediction – Demand Forecasting Model

Goal:
Forecast future ride demand trends based on time, day, and weather.

Model: Time Series (ARIMA / LSTM)
Inputs: date, time_of_day, weather, traffic_level, avg_fare
Outputs: predicted_rides

KPIs:

Forecast Accuracy (%)

Demand Peaks by Day/Time

Weather Impact Index

Visuals:

Demand Trend Over Time

Day-Time Heatmap

Hourly Ride Pattern Chart

📊 Key Insights Across All Use Cases
Category	Observation
Dynamic Pricing	Fare increases under high demand & bad weather
Route Optimization	Highways are most efficient & predictable
Fast Matching	Low traffic = faster matches
Fraud Detection	High fare & low driver rating = fraud risk
Ride Prediction	Weekends & rainy days drive higher demand
🧠 Future Enhancements

Integrate real-time API data streams (e.g., Uber Movement, OpenWeatherMap).

Implement real-time dashboards using Dash or Streamlit.

Add automated model retraining with Databricks Jobs or GitHub Actions.

Deploy models as APIs for live predictions.

🏁 Conclusion

This project consolidates five major data analytics applications under a unified Big Data pipeline, proving how insights from data can improve pricing strategies, route planning, driver efficiency, fraud control, and demand forecasting in the transportation industry.

🧾 License
