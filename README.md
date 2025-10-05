# 🐦 Bird Biodiversity Trends in North America (2000–2024)

## 📘 Overview
This project analyzes bird biodiversity across the United States, Canada, and Mexico using the **Global Biodiversity Information Facility (GBIF)** dataset.  
The analysis explores:
1. **Geographic shifts in bird species over time**  
2. **Changes in biodiversity across regions**  
3. **Patterns in record types** (e.g., citizen science vs. institutional records)

This study was completed as part of the DSC680 course at Bellevue University and uses data-driven methods to better understand ecological trends across North America.

---

## 📊 Data Source
- **Dataset:** `bigquery-public-data.gbif.occurrences` (GBIF on Google BigQuery)  
- **Data Period:** 2000–2024  
- **Filters Applied:**  
  - `class = 'Aves'`  
  - `year BETWEEN 2000 AND 2024`  
  - `countryCode IN ('US', 'CA', 'MX')`  
  - Valid geographic coordinates (`decimalLatitude` and `decimalLongitude` not null)

---

## 🧰 Methods
- **Querying:** SQL via Google BigQuery  
- **Processing:** Python (`pandas`, `matplotlib`, `seaborn`, `statsmodels`)  
- **Analysis Techniques:**  
  - Species richness counts and diversity comparisons  
  - Trend and regression analysis  
  - Temporal and spatial visualizations  
- **Visualization Tools:** Matplotlib, Seaborn

---

## 🔍 Key Findings
- 🇺🇸 The **United States** holds the highest **total species richness** across the dataset.  
- 🇲🇽 **Mexico** shows greater **species variety per observation**, indicating localized biodiversity.  
- 🇨🇦 **Canada’s** records, particularly in Quebec, show steady participation but limited diversity compared to southern regions.  
- **Citizen science submissions** have increased sharply after 2015, dominating record counts.  
- Geographic patterns show **limited northward movement** in bird distribution overall.  
- Biodiversity hotspots are concentrated in **California, Texas, and Quebec**.

---

## ⚙️ How to Reproduce
1. **Clone the repository**
   ```bash
   git clone https://github.com/YOURUSERNAME/bird-biodiversity-dsc680.git
   cd bird-biodiversity-dsc680
