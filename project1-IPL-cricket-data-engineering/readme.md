# 🏏 IPL Data Engineering Project

## 📋 Project Overview
This project is focused on performing **data engineering and analytics** on IPL (Indian Premier League) data using **PySpark**. The goal is to process, clean, and analyze IPL datasets to generate insights into player performance, match statistics, and team trends. The project includes data ingestion from **Amazon S3**, transformation, and SQL-based queries using Spark.

---

## 📂 Project Structure
The repository contains the following key components:
```text
|-- data        # S3 bucket
|-- notebooks   # Jupyter Notebooks with project code
|-- README.md   # Project documentation (this file)
```

---

## ⚙️ Technologies Used
- **PySpark**: For distributed data processing and analytics
- **Databricks**: For running notebooks and queries
- **Amazon S3**: For storing and accessing datasets
- **Python**: For data preprocessing and transformations

---

## 📊 Features
1. **Data Ingestion**:
   - Load IPL datasets (e.g., matches, players, ball-by-ball data) from an Amazon S3 bucket into Spark DataFrames.
   
2. **Data Transformation**:
   - Clean and preprocess data (e.g., handling null values, normalizing player names).
   - Create additional columns for detailed analysis (e.g., `batting_style`, `win_margin_category`).

3. **Data Analysis Using Spark SQL**:
   - Perform SQL queries on the IPL data for:
     - Identifying top-performing players.
     - Analyzing team trends.
     - Calculating win margins and toss effects.

4. **Custom Insights**:
   - Generate insights such as:
     - Highest-scoring batsmen per season.
     - Impact of toss on match outcomes.
     - Categorization of wins based on margin.

---

## 🗂️ Datasets
The datasets used in this project are stored in an **Amazon S3 bucket**. Below are the tables created during the analysis: 
- `match.csv`: Match-level data (teams, dates, venue, season year, etc.).
- `players.csv`: Player-level data (player name, batting hand, bowling skill, country).
- `ball_by_ball.csv`: Ball-level data (runs scored, dismissals, and match context).
- `player_match`: Links players to specific matches (match_id,player_id,team_id).
- `team`: Team information including team names and identifiers. (team_id,team_name).  
 
You need to store and use your s3 bucket for accessing the data s3a://your-private-bucket/datasets.csv


