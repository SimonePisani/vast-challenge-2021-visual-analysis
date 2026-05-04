# VAST Challenge 2021 – Interactive Visual Analytics System

An interactive visual analytics system designed to explore, analyze and uncover patterns, anomalies and relationships in a complex multi-source dataset (GPS, credit card, and loyalty transactions).

The project integrates **temporal, geospatial and relational visualizations** to support investigative analysis across different days, locations and entities.

Originally developed as part of a Visual Analytics course, this project focuses on transforming raw, inconsistent data into meaningful insights through interactive exploration.

---

## Problem & Goals

The dataset contains heterogeneous and partially inconsistent data sources, including:

* GPS traces of individuals
* Credit card transactions
* Loyalty card transactions
* Employee and vehicle assignments

The goal of the project is to support analytical tasks such as:

* Identifying the most popular locations and their temporal patterns
* Detecting anomalies in transactional behavior
* Inferring relationships between individuals
* Correlating movements with financial activity
* Highlighting potential suspicious behaviors

---

## Analytical Process

The project follows a structured visual analytics workflow based on progressive exploration:

1. **Overview Phase**

   * Identify global patterns across locations and days
   * Highlight high-density transactional areas

2. **Focused Analysis**

   * Apply filters (location, day, time)
   * Explore distributions, price variations and payment methods

3. **Relational Exploration**

   * Analyze connections between time, price and transaction types
   * Identify correlations and anomalies

4. **Geospatial Investigation**

   * Track movements of individuals over time
   * Correlate mobility with transactional activity
   * Detect inconsistencies and suspicious patterns

---

## Data Preparation & Engineering

The original dataset presented several challenges:

* Inconsistent timestamp formats across sources
* Non-unique identifiers (e.g. last 4 digits of credit cards)
* Large dataset size

To address these issues:

* Converted CSV datasets into JSON format
* Transformed geospatial data into **GeoJSON** for D3 integration
* Merged GPS and car assignment data using the `id` field
* Cleaned and reduced dataset size by removing non-essential fields
* Normalized timestamps for consistent temporal analysis

This preprocessing phase was essential to enable meaningful cross-dataset analysis.

---

## Visualizations & System Design

The system is structured into three main analytical layers:

### 1. Overview (Global Patterns)

* **Heatmap** → transaction density across locations and days
* **Statistical summary** → total, mean, mode, standard deviation

Provides a quick and intuitive understanding of overall trends.

---

### 2. Focused Analysis (Filtered Insights)

* Interactive filters (location, day)
* Coordinated visualizations:

  * **Bar chart** → transactions by hour
  * **Pie chart** → payment method distribution
  * **Scatterplot** → price peaks and variations
  * **Sankey diagram** → relationships between time, price and payment methods

The Sankey diagram was introduced to better represent multi-variable relationships not clearly visible in simpler charts.

---

### 3. Geospatial Analysis (Behavioral Patterns)

* Interactive map with movement tracking
* Time-based controls (forward/backward timeline)
* Movement trails highlighting recent paths
* Dynamic updates of transactions and movements

Designed to correlate spatial behavior with financial activity.

---

## Key Insights

The system enables:

* Identification of the most active locations and their temporal patterns
* Detection of transaction anomalies and unusual peaks
* Correlation between movement and financial activity
* Exploration of potential relationships between individuals
* Identification of inconsistencies between GPS, credit and loyalty data

The combination of multiple coordinated views allows deeper investigation compared to isolated visualizations.

---

## Tech Stack

* **Frontend:** Vue.js
* **Visualization:** D3.js
* **Data Processing:** JavaScript / JSON / GeoJSON

---

## Project Structure

```
src/
 ├── components/       # Visualization components (heatmap, map, sankey, etc.)
 ├── assets/           # Data and static resources
 ├── App.vue
 └── main.js
```

---

## How to Run

```bash
npm install
npm run serve
```

---

## Notes

* This project was originally developed in a university environment and later consolidated into this repository
* The commit history does not fully reflect the original development process

---

## Future Improvements

* Deploy interactive demo
* Optimize performance for large datasets
* Improve UI/UX for better usability
* Add automated data preprocessing pipeline

---

## Screenshots / Demo

Overview
<img width="1845" height="879" alt="Screenshot 2026-05-04 100530" src="https://github.com/user-attachments/assets/cef82329-05b2-445a-96d7-9a58773549c6" />

---

Focused View
<img width="1834" height="864" alt="Screenshot 2026-05-04 100558" src="https://github.com/user-attachments/assets/ecbfcbd3-be3f-4086-aba2-de5fc9564991" />

---

Geospatial Map
<img width="1853" height="876" alt="Screenshot 2026-05-04 100639" src="https://github.com/user-attachments/assets/2e238ca2-1bff-44c0-be8d-2666e7c43838" />

