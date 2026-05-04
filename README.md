# VAST Challenge 2021 – Visual Analysis

Interactive web-based visual analytics project focused on anomaly detection and pattern exploration using the VAST Challenge 2021 dataset.

---

## 🚀 Overview

This project explores the VAST Challenge 2021 (Mini Challenge 2) dataset through interactive visualizations.

The application provides tools to analyze transactions, movement data, and geospatial information, enabling users to identify patterns, anomalies, and relationships within the dataset.

The system is designed as an exploratory analysis tool, combining multiple coordinated views to support data-driven insights.

---

## ✨ Features

* 📊 Interactive data visualizations
* 🔥 Heatmap of transactions over time and locations
* 🔗 Sankey diagram for transaction relationships
* 📈 Statistical indicators (mean, mode, standard deviation)
* 🕒 Temporal analysis (transactions per hour/day)
* 🗺️ Geospatial visualization of movements
* 🎯 Focused analysis views per location and time
* 🔍 Pattern and anomaly detection support

---

## 🧠 Analysis Goals

The project focuses on:

* Identifying high-activity locations
* Detecting temporal patterns in transactions
* Analyzing differences between credit and loyalty card usage
* Exploring relationships between entities through movement data
* Highlighting anomalies and unusual behaviors

---

## 🛠️ Tech Stack

* Vue.js
* JavaScript
* D3.js (data visualization)
* HTML / CSS

---

## 📁 Project Structure

```text
.
├── public/                         # Static assets
├── src/                            # Main application source code
│   ├── components/                 # Visualization components
│   ├── views/                      # Main views
│   ├── assets/                     # Dataset and resources
│   └── main.js                     # App entry point
│
├── package.json                    # Dependencies and scripts
├── vue.config.js                   # Vue configuration
└── README.md
```

---

## ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/SimonePisani/vast-challenge-2021-visual-analysis.git
cd vast-challenge-2021-visual-analysis
```

Install dependencies:

```bash
npm install
```

---

## ▶️ Usage

Run the development server:

```bash
npm run serve
```

Then open:

```
http://localhost:8080
```

---

## 📊 Dataset

Full dataset available at:
https://vast-challenge.github.io/2021/MC2.html

---

## 📷 Visualizations

The system provides multiple coordinated views:

* Heatmap overview of transactions
* Detailed focus view with statistical analysis
* Sankey diagram for transaction flow
* Geospatial movement visualization

---

## 📌 Notes

This project focuses on exploratory data analysis and visualization techniques applied to a complex real-world dataset.

---

## 🚧 Future Improvements

* Improve performance with large datasets
* Add filtering and brushing interactions
* Enhance UI/UX for better usability
* Deploy as a hosted web application

---

## 👨‍💻 Author

Simone Pisani
