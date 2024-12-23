
# README: Berlin Traffic Prediction and Autonomous Vehicle Route Optimization

## Overview
This project predicts traffic congestion in Berlin and optimizes routes for autonomous vehicles using integrated data from multiple sources and advanced machine learning techniques. It aims to improve traffic flow, reduce travel times, and minimize fuel consumption.

---

## Objectives
1. **Traffic Prediction**:
   - Develop models to forecast traffic density and speed.
2. **Route Optimization**:
   - Suggest optimal routes for autonomous vehicles.
3. **Efficiency Improvement**:
   - Shorten travel times.
   - Reduce fuel consumption.
   - Improve overall traffic flow.

---

## Data Sources
This project leverages multiple data sources for comprehensive analysis:

1. **Traffic Data**:
   - **Source**: Berlin Municipality Traffic Management.
   - **API**: [Berlin Traffic Detection API](https://api.viz.berlin.de/daten/verkehrsdetektion)
   - **Description**: Provides hourly traffic flow and congestion data.

2. **Weather Data**:
   - **Source**: Open-Meteo.
   - **API**: [DWD Weather API](https://open-meteo.com/en/docs/dwd-api#latitude=52.5244&longitude=13.4105)
   - **Description**: Real-time and historical weather data, including temperature, wind, and precipitation.

3. **Public Transportation Data**:
   - **Source**: Berliner Verkehrsbetriebe (BVG).
   - **API**: [VBB GTFS Data](https://daten.berlin.de/datensaetze/vbb-fahrplandaten-via-gtfs)
   - **Description**: Public transportation schedules and route information.

4. **Road and Construction Data**:
   - **Source**: Berlin Municipality.
   - **API**: [Berlin Construction API](https://api.viz.berlin.de/daten/verkehrsdetektion)
   - **Description**: Information on roadworks and ongoing construction projects.

---

## Methodology
1. **Data Integration**:
   - Merge traffic, weather, holiday, and construction data into a unified dataset.
   - Perform feature engineering to create variables like `is_weekend` and `is_under_construction`.

2. **Exploratory Data Analysis (EDA)**:
   - Analyze the impact of holidays, weather, and construction on traffic patterns.
   - Visualize correlations, spatial data, and temporal trends using heatmaps and scatter plots.

3. **Machine Learning Models**:
   - Train models such as:
     - Random Forest
     - CatBoost
     - XGBoost
     - Neural Networks
   - Compare performance using metrics like MSE (Mean Squared Error) and R².

4. **Clustering**:
   - Use K-Means clustering to identify traffic patterns and hotspots.

5. **Optimization**:
   - Predict traffic density and recommend optimal routes for autonomous vehicles.

---

## Key Features
- **Integrated Data Sources**:
  - Combines traffic, weather, public transportation, and construction data.
- **Advanced Machine Learning Models**:
  - Implements state-of-the-art algorithms for prediction and optimization.
- **Comprehensive Visualizations**:
  - Includes spatial, temporal, and scenario-based analyses.
- **Scalable Framework**:
  - Easily extendable to other cities or data sources.

---

## Installation
To run this project locally:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/username/berlin-traffic-analysis.git
   ```

2. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Jupyter Notebook**:
   ```bash
   jupyter notebook berlin_traffic_analysis.ipynb
   ```

---

## Results
1. **Best Performing Model**: Random Forest with R² of 0.772.
2. **Holiday Insights**: Traffic speeds are slightly higher on holidays due to reduced congestion.
3. **Spatial Insights**: Traffic density is highest in central Berlin.

---

## Future Directions
- Incorporate real-time traffic data for dynamic predictions.
- Extend the model to other cities with similar data availability.
- Integrate real-time public transportation delays into predictions.

---

## Contributing
Contributions are welcome! To contribute:
1. Fork the repository.
2. Create a new branch for your feature.
3. Submit a pull request with detailed explanations.

---

## License
This project is licensed under the MIT License.

