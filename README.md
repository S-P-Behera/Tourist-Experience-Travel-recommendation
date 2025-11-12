# 🌍 Tourist Experience & Travel Risk Analysis System  

## 📘 Project Overview  
This project aims to analyze and enhance the understanding of tourist experiences and travel safety across major destinations in India. Using **Big Data Analytics**, **PySpark**, and **Natural Language Processing (NLP)** in **Databricks**, this system extracts valuable insights from large-scale traveler reviews to assess ratings, sentiments, risk levels, traveler preferences, and more.  

The final outcome includes a **data pipeline (Bronze–Silver–Gold layers)**, **seven analytical use cases**, and an **interactive dashboard** for decision-making in tourism management and policy improvement.  

---

## 🎯 Objectives  
- Analyze tourist feedback data to identify travel satisfaction trends.  
- Perform sentiment and safety risk analysis using NLP.  
- Build PySpark pipelines to handle large datasets efficiently.  
- Generate actionable insights to guide travelers and tourism authorities.  
- Visualize the results using dashboards for intuitive interpretation.  

---

## 🧠 Technologies Used  
| Category | Tools / Libraries |
|-----------|------------------|
| Platform | Databricks (Apache Spark) |
| Language | Python (PySpark, Pandas) |
| NLP | NLTK (VADER Sentiment Analysis) |
| Visualization | Databricks Dashboard |
| Data Storage | Delta Lake Architecture (Bronze → Silver → Gold) |
| File Format | CSV (Tourist Experience Dataset – India) |

---

## 🧩 Data Pipeline Architecture  
The project follows the **Medallion Architecture** (Bronze, Silver, and Gold layers):  

- **Bronze Layer** → Raw data ingestion and schema definition.  
- **Silver Layer** → Data cleaning, transformation, and NLP processing.  
- **Gold Layer** → Analytical data models and dashboards for visualization.  

---

## 📊 Use Cases Implemented  

### 🏙️ 1. Tourist Rating Analysis by City  
**Goal:** Identify top-rated and lowest-rated tourist destinations.  
**Methodology:** Grouped and averaged ratings using PySpark aggregation.  
**Output:** Ranked list of cities by average tourist rating.

---

### 💬 2. Sentiment Analysis of Tourist Reviews  
**Goal:** Understand traveler emotions (Positive, Negative, Neutral).  
**Methodology:** Applied VADER SentimentIntensityAnalyzer from NLTK on review texts.  
**Output:** Sentiment scores and sentiment labels for each review.

---

### 🚨 3. City Safety & Travel Risk Score  
**Goal:** Determine which destinations are safer or riskier.  
**Methodology:** Combined negative sentiment ratios with average ratings to compute a custom `risk_score`.  
**Output:** Categorized cities into “Safe,” “Moderate Risk,” and “High Risk.”

---

### 🌦️ 4. Best Travel Season Recommendation  
**Goal:** Recommend the best months and seasons for travel.  
**Methodology:** Combined ratings and sentiment to calculate an `experience_score` and classified months by quartile thresholds.  
**Output:** Seasonal travel recommendations — “Highly Recommended,” “Good Time,” etc.

---

### 👥 5. Traveler Type Profiling  
**Goal:** Understand which types of travelers enjoy which destinations.  
**Methodology:** Grouped by `traveler_type` and `city` to compute average rating.  
**Output:** Mapped traveler profiles with preferred destinations (e.g., Family → Pondicherry, Solo → Bengaluru).

---

### 🏞️ 6. Top 10 Most Loved Attractions  
**Goal:** Identify the most popular tourist attractions in India.  
**Methodology:** Aggregated experience scores by attraction name and sorted top 10.  
**Output:** List of top attractions with highest satisfaction levels.

---

### ⚠️ 7. Complaint & Pain Point Mining  
**Goal:** Identify common tourist complaints using NLP keyword extraction.  
**Methodology:** Tokenized reviews, extracted high-frequency negative keywords (e.g., crowd, expensive, scam), and mapped to descriptive insights.  
**Output:** City-wise dominant complaints for tourism improvement.

---

## 🧮 Methodology Summary  

1. **Data Ingestion (Bronze Layer)**  
   - Loaded raw CSV data into Databricks Delta tables.  

2. **Data Cleaning & NLP (Silver Layer)**  
   - Removed missing values and irrelevant records.  
   - Applied NLP using NLTK’s VADER for sentiment scoring.  

3. **Analytical Modeling (Gold Layer)**  
   - Created PySpark models for each use case.  
   - Computed ratings, risk levels, and seasonal scores.  

4. **Visualization & Insights**  
   - Built an interactive Databricks dashboard with charts such as bar graphs, area plots, pie charts, and heatmaps.  
   - Showcased tourist satisfaction, seasonality trends, and complaint hotspots.

---

## 📈 Key Insights  

- **Delhi**, **Mumbai**, and **Goa** show high traveler volume but varying satisfaction due to crowd and cost factors.  
- **Pondicherry**, **Ooty**, and **Jaipur** stand out for consistent positive experiences.  
- **Monsoon season** yields moderate satisfaction; **winter months** are most preferred for travel.  
- **Family** and **Couple travelers** report higher satisfaction compared to **solo travelers**.  
- Common pain points include **crowding**, **high prices**, and **cleanliness issues**.

---

## 📊 Dashboard Overview  
The dashboard provides:  
- **City-wis**
