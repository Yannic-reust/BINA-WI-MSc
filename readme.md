# Veloinfrastruktur in Bern: A Data-Driven CPA Analysis

## 📌 Overview
**Where is additional, safe bicycle infrastructure most urgently needed in Bern?**

As the city of Bern pursues its "Velo-Offensive" to increase the share of cycling from 11% to 20%, a critical question remains: despite increased investment, accidents continue to occur. This project moves beyond speculation by using spatial data science to identify specific accident hotspots. By analyzing over a decade of accident statistics (2014–2025) and traffic indices, this analysis provides a data-backed priority list for urban planners.

## 🚀 Key Findings
* **Safety Trend:** While bicycle traffic in Bern has increased by approximately 80% since 2014, accident numbers have remained stable or even decreased since 2019, suggesting that recent measures are working.
* **Hotspot Identification:** The spatial analysis identified 17 critical accident concentrations (hotspots) within the city limits.
* **Infrastructure Focus:** High-risk areas are concentrated around major transit arteries (e.g., near Bahnhof and Kornhaus).
* **Evidence of Success:** Case studies of recent interventions (e.g., Haltestelle Wander and Lorrainebrücke) show a measurable reduction in accident frequency per year following structural changes.

## 🛠 Methodology: The CPA Process
This project follows the **CPA (Challenge, Process, Answer)** framework to ensure actionable insights:

* **Challenge:** Define the problem of identifying infrastructure gaps amidst rising traffic volumes.
* **Process:**
    * **Data Collection:** Integrating official AESTRA accident datasets and Bern city traffic indices.
    * **Spatial Analysis:** Implementing a 250m x 250m grid-based spatial join to identify statistical clusters.
    * **Temporal Analysis:** Comparing accident rates against the growth of cycling-index over time.
* **Answer:** Providing an interactive Folium map and a prioritized list of hotspots for decision-makers.

## 📊 Tech Stack
* **Language:** `Python`
* **Geospatial Analysis:** `GeoPandas`, `Shapely`, `OSMnx`
* **Visualization:** `Folium` (Interactive Maps), `Matplotlib`, `Seaborn`, `Contextily` (Basemaps)
* **Data Manipulation:** `Pandas`, `NumPy`
* **Statistical Analysis:** `SciPy` (Linear Regression & Quantile-based Hotspot detection)

## 📂 Data Sources
* **ASTRA (Federal Roads Office):** Official accident statistics with person injuries via [data.geo.admin.ch](https://data.geo.admin.ch).
* **Stadt Bern:** Annual bicycle traffic indices and infrastructure project data.

## 📖 How to Use this Notebook
1. Open the file in **Google Colab**.
2. Run all cells sequentially.
3. **Note:** The notebook is designed to automatically attempt a download of the ASTRA dataset. If the official URL changes, please follow the manual download instructions provided in the "Data Collection" cell.

## ⚠️ Limitations
* **Reporting Bias:** Data only includes accidents reported to the police (excludes minor accidents without injuries).
* **Infrastructure Context:** The analysis identifies where accidents happen but does not explicitly map every existing bike lane due to inconsistencies in OpenStreetMap tagging; instead, it uses accident density as a proxy for infrastructure gaps.

## 👥 Authors
* Lukas Küng
* Yannic Reust
* Ahimsa Romero
* Dario Schai
* Joel Schwarz

**Project Date:** June 2, 2026
