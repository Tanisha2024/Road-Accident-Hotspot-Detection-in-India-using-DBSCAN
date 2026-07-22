# 🚦 Road Accident Hotspot Detection in India using DBSCAN

## 📌 Project Overview

Road accidents are a major public safety concern in India. Identifying accident-prone locations (hotspots) helps government agencies and traffic authorities prioritize road safety measures, improve infrastructure, and reduce accidents.

This project applies the **DBSCAN (Density-Based Spatial Clustering of Applications with Noise)** algorithm to identify accident hotspots using GPS coordinates (latitude and longitude). The results are compared with **K-Means Clustering** to demonstrate why DBSCAN is more suitable for geospatial hotspot detection.

---

# 🎯 Problem Statement

The objective of this project is to identify accident hotspots across India using GPS location data and analyze accident patterns based on:

* Location
* Accident Severity
* Traffic Density
* Weather Conditions
* Risk Score

The project also detects isolated accidents (outliers) that do not belong to any hotspot.

---

# 📂 Dataset

The dataset contains approximately **20,000 road accident records** across India.

### Features Used

| Feature           | Description          |
| ----------------- | -------------------- |
| latitude          | Accident Latitude    |
| longitude         | Accident Longitude   |
| city              | City Name            |
| state             | State Name           |
| accident_severity | Severity of Accident |
| weather           | Weather Condition    |
| traffic_density   | Traffic Density      |
| risk_score        | Accident Risk Score  |

---

# 🛠 Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* Folium
* Jupyter Notebook

---

# 📊 Exploratory Data Analysis (EDA)

The following analyses were performed before clustering:

### Univariate Analysis

* Accident Severity Distribution
* Weather Distribution
* Traffic Density Distribution
* State-wise Accident Count
* City-wise Accident Count
* Risk Score Distribution

### Bivariate Analysis

* Weather vs Accident Severity
* Traffic Density vs Accident Severity
* Road Type vs Accident Severity
* Time of Day vs Accident Severity
* Correlation Analysis
* GPS Scatter Plot

---

# 🤖 Machine Learning

## DBSCAN

The project uses **DBSCAN** to identify accident hotspots based on GPS coordinates.

### Parameters

* Metric: Haversine Distance
* eps: 2 km
* min_samples: 10

### Why Haversine Distance?

Latitude and longitude represent locations on the Earth's surface. Haversine distance calculates the shortest distance between two GPS coordinates and is more accurate than Euclidean distance for geospatial data.

---

# 📍 Workflow

1. Import Libraries
2. Load Dataset
3. Data Cleaning
4. Exploratory Data Analysis
5. GPS Visualization
6. Convert Coordinates to Radians
7. Apply DBSCAN
8. Detect Hotspots
9. Detect Outliers
10. Compare with K-Means
11. Interactive Folium Map
12. Business Insights

---

# 📈 Results

The DBSCAN algorithm successfully identified dense accident hotspots and isolated accident locations.

### DBSCAN

✅ Automatically determines clusters

✅ Detects accident hotspots

✅ Detects isolated accidents as noise

✅ Works well with irregular cluster shapes

---

### K-Means

* Requires predefined number of clusters
* Cannot detect outliers
* Forces every accident into a cluster
* Less suitable for geospatial hotspot detection

---

# 📍 Interactive Map

An interactive map was created using **Folium**.

Features:

* Zoomable map
* Cluster visualization
* Color-coded hotspots
* Accident location markers
* Pop-up information
* Accident Heatmap

---

# 📊 Business Insights

* Identified high-density accident hotspots across India.
* Detected isolated accident locations that may require separate investigation.
* Compared hotspot characteristics using accident severity and risk score.
* Analyzed the relationship between weather, traffic density, and accident severity.
* Demonstrated that DBSCAN is more effective than K-Means for GPS-based clustering.

---


# 🚀 Future Improvements

* Real-time accident hotspot monitoring
* Integration with live traffic APIs
* Streamlit dashboard deployment
* Predictive accident risk modeling
* Time-series hotspot analysis
* Route safety recommendation system

---

# 📚 Learning Outcomes

Through this project, I learned:

* Data Cleaning
* Exploratory Data Analysis
* Geospatial Data Processing
* DBSCAN Clustering
* Haversine Distance
* Outlier Detection
* K-Means Clustering
* Interactive Mapping using Folium
* Machine Learning Workflow
* Business Insight Generation

---

# 🙌 Acknowledgements

* Scikit-learn Documentation
* Folium Documentation
* Python Open Source Community

---

## ⭐ If you found this project useful, consider giving it a star on GitHub!
