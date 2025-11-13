# Air Pollution Analytics and Forecasting in Indian Cities


This project analyzes large-scale air quality data from Indian cities to identify **pollution trends**, **dominant pollutants**, and **seasonal variations**.  
Developed using **Apache PySpark** for distributed data processing and **Matplotlib** for visualization, it also employs a **SARIMA model** for forecasting future AQI levels.  
The insights generated support **environmental planning**, **policy formulation**, and **public health protection**.

# Features

# Data Cleaning & Preprocessing
• Handled missing values and standardized column names.
• Converted date columns and extracted temporal features (month, year, season).

# Exploratory Data Analysis (EDA)
• Computed average AQI (Air Quality Index) by city, month, and year.
• Identified top 5 polluted cities for each major pollutant (PM2.5, PM10, NO₂, SO₂, CO, O₃).
• Analyzed seasonal pollution trends (Winter, Summer, Monsoon, Post-Monsoon).
# 🌡 Heatmap Analysis  
- Generated **heatmaps** to identify air pollution hotspots across India.  
- Visualized pollution intensity city-wise and season-wise using **Folium**.  

# Forecasting (SARIMA Model)  
- Applied **Seasonal AutoRegressive Integrated Moving Average (SARIMA)** model *(1,1,1)(1,1,1,12)*.  
- Forecasted **10-day AQI trends** for top polluted cities and the national average.  
- Predicted AQI levels remain in the **“Poor” to “Very Poor”** range, highlighting ongoing pollution concerns.  


# Visualization
• Line and bar plots showing monthly, yearly, and seasonal trends.
• AQI level categorization (Good → Severe).

 # Technologies Used

Apache PySpark — distributed data processing

Matplotlib / Pandas — visualization and summary statistics

Jupyter / Colab — interactive development environment

# Dataset

The dataset city_day.csv contains daily air quality metrics across Indian cities, including:

Date and city

Pollutant concentrations (PM2.5, PM10, NO₂, SO₂, CO, O₃)

Air Quality Index (AQI)



# Setup & Execution

Clone the Repository

git clone https://github.com/<your-username>/india-air-quality-analysis.git
cd india-air-quality-analysis


Install Dependencies

pip install pyspark pandas matplotlib


Run the Script

python air_quality_analysis.py


# Output

Aggregated AQI statistics by city, month, and season


Line and bar plots for temporal and seasonal analysis

📈 Sample Visuals

Monthly Air Quality Trends — variation of AQI across months.

Yearly Pollution Trend — long-term progression in air quality.

Seasonal AQI Comparison — seasonal differences in air quality.

Heatmap of Polluted Regions — spatial distribution of AQI levels.

🧾 Insights

Delhi, Kolkata, and Mumbai consistently have the highest PM2.5 levels.

Winter months record the poorest air quality due to temperature inversion and increased emissions.

Heatmaps highlight pollution hotspots in industrial and urban areas.

Forecasting shows that AQI remains in the Poor–Very Poor range for the next 10 days.

PM2.5 and PM10 remain the key pollutants influencing AQI levels.
# 💡 Future Enhancements

Integrate real-time AQI APIs for live updates.

Add meteorological factors (temperature, humidity, wind speed).

Build an interactive dashboard using Streamlit or Plotly Dash.

Extend forecasting using LSTM or Prophet models for improved accuracy.
