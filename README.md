# 🚦 Toronto Collision Severity Analysis (Big Data Project)

## 📌 Overview
This project analyzes traffic collision data from the Toronto Open Data Portal to identify environmental and road-related factors influencing accident severity.

Using Apache Spark, Spark Structured Streaming, and MongoDB Atlas, the project demonstrates a full big data pipeline — from ingestion and data quality processing to analytics, streaming simulation, and storage.

## ⚙️ Tech Stack
- Apache Spark (PySpark)
- Spark Structured Streaming
- Python
- MongoDB Atlas
- Parquet
- Matplotlib

## 📊 Dataset
- Source: Toronto Open Data Portal
- Records: ~20,000 collision records (2006–2025)
- Features include:
  - Collision severity
  - Lighting conditions
  - Road surface conditions
  - Impact types
  - Time and location data

## 🧹 Data Quality & Processing
- Removed irrelevant columns with high missing values
- Dropped nulls in key analytical variables
- Validated data integrity (no duplicates found)
- Reduced dataset from 20,419 → 19,718 records
- Performed feature engineering (year, month, hour, day of week)

## 🔍 Key Insights
- **85.99%** of collisions were non-fatal, while **13.92%** were fatal :contentReference[oaicite:1]{index=1}  
- Low-light conditions (dusk, dawn, night) showed higher fatality rates  
- Hazardous road conditions (e.g., packed snow) had disproportionately higher fatal outcomes  
- Peak collision volume occurred in summer months (June–August)  
- Nighttime collisions, though fewer, had higher severity  

## ⚡ Streaming Simulation
- Simulated real-time data ingestion using Spark Structured Streaming
- Processed yearly data as micro-batches
- Verified pipeline with total processed count of **19,718 records**

## 🗄️ Data Storage
- Stored outputs in:
  - Parquet files (local backup)
  - MongoDB Atlas (NoSQL collections)

## 📈 Visualizations
- Collision severity distribution
- Lighting condition analysis
- Road surface impact analysis
- Time-series trends
- Monthly heatmaps
- High-risk neighbourhood analysis

## 📁 Files
- `notebook.ipynb` → Full implementation
- `report.pdf` → Detailed project report

## 🚀 Key Takeaway
This project demonstrates how big data tools can be used to transform raw transportation data into actionable insights for urban planning, policy-making, and road safety improvement.

---