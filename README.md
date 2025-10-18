# Unveiling India’s Air Pollution Patterns Through Pyspark Analysis 

This project analyzes large-scale air quality data from Indian cities to identify pollution trends, major contributing pollutants, and seasonal or temporal patterns. Built using PySpark for scalable data processing and Matplotlib for visualization, the analysis provides insights to support environmental planning and public health policy.

Features

Data Cleaning & Preprocessing
• Handled missing values and standardized column names.
• Converted date columns and extracted temporal features (month, year, season).

Exploratory Data Analysis (EDA)
• Computed average AQI (Air Quality Index) by city, month, and year.
• Identified top 5 polluted cities for each major pollutant (PM2.5, PM10, NO₂, SO₂, CO, O₃).
• Analyzed seasonal pollution trends (Winter, Summer, Monsoon, Post-Monsoon).

Correlation Analysis
• Calculated pollutant correlations to study co-variability and pollutant interactions.

Visualization
• Line and bar plots showing monthly, yearly, and seasonal trends.
• AQI level categorization (Good → Severe).

 Technologies Used

Apache PySpark — distributed data processing

Matplotlib / Pandas — visualization and summary statistics

Jupyter / Colab — interactive development environment

Dataset

The dataset city_day.csv contains daily air quality metrics across Indian cities, including:

Date and city

Pollutant concentrations (PM2.5, PM10, NO₂, SO₂, CO, O₃)

Air Quality Index (AQI)

You can download the dataset from the Kaggle: Air Quality Data in India (2015–2020)
 source.

Setup & Execution

Clone the Repository

git clone https://github.com/<your-username>/india-air-quality-analysis.git
cd india-air-quality-analysis


Install Dependencies

pip install pyspark pandas matplotlib


Run the Script

python air_quality_analysis.py


Output

Aggregated AQI statistics by city, month, and season

Correlation heatmap data between pollutants

Line and bar plots for temporal and seasonal analysis

📈 Sample Visuals

Monthly Air Quality Trends

Yearly Pollution Trend

Seasonal AQI Comparison

🧾 Insights

Delhi, Kolkata, and Mumbai show the highest PM2.5 levels.

AQI peaks during winter months due to stagnant weather and increased emissions.

PM2.5 and PM10 show strong correlation with AQI, indicating their dominant influence on overall air quality.
