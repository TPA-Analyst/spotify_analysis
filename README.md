# End-to-End Spotify Listening History Analytics

[![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-yellow.svg)](https://powerbi.microsoft.com/)
[![DAX](https://img.shields.io/badge/DAX-Queries-blue.svg)](https://dax.guide/)
[![Gamma](https://img.shields.io/badge/Gamma%20App-Presentation-purple.svg)](https://gamma.app/)

---

## 📌 Project Overview
This end-to-end data analytics project focuses on performing comprehensive analysis using Spotify history data to visualize listening trends over time, identify top-performing content, and calculate year-on-year growth.

The primary objective is to implement quadrant analysis to categorize tracks based on listening frequency and duration, translating raw listening behaviors into actionable business insights for marketing and pricing.

---

## 📁 Dataset Architecture
The dataset contains 149,861 high-quality, pre-cleaned records with 11 key features representing user listening history. Key columns include:
- **`track_uri`**: *Unique identifier for each Spotify track.*
- **`TS`** / **`timestamp`**: *Specific timestamps for listening sessions.*
- **`platform`**: *The device or platform used for the listening session.*
- **`track_name`** / **`artist_name`** / **`album_name`**: *Essential metadata identifying the music.*
- **`shuffle`**: *Usage metric indicating whether shuffle mode was active.*
- **`skipped`**: *Usage metric capturing skip events to evaluate user engagement and drop-off rates.*

---

## 🛠️ Tools & Technologies
- **Power BI**: *Data Preparation (Power Query), Data Modeling, and interactive Dashboard visualization.*
- **DAX Studio**: *Writing and optimizing complex Data Analysis Expressions (DAX) queries.*
- **Gamma**: *Generating the final professional presentation for stakeholders.*

---

## 🚀 Steps & Methodology
1. **Exploratory Data Analysis (EDA) & Cleaning**: Utilized Power Query Editor to perform ETL operations and ensure data quality (resolving 2 error values, 0 missing data).
2. **Data Modeling**: Established a one-to-many relationship between the Spotify history table and a custom Date Table to enable Time Intelligence functions.
3. **DAX Calculations**: Created advanced measures for YoY performance, MIN/MAX logic for line charts, and complex quadrant logic.
4. **Dashboard Development**: Built an interactive Power BI dashboard featuring drill-through, drill-down, and hierarchical navigation.

---

## 📊 Dashboard & Insights
The interactive dashboard includes several key views:
- **Performance KPIs**: Tracks the latest year versus previous year listening metrics for tracks, albums, and artists.
- **Trend Visuals**: Dynamically displays peak and lowest listening periods over time.
- **Quadrant Analysis**: Evaluates average listening time against track frequency to isolate the most engaging content.
- **Granular Exporting**: Allows users to export specific, detailed data directly to stakeholders.

---

## 💡 Business Recommendations
- **Marketing Adjustments**: Increase marketing spend to boost user engagement if specific albums show a decreasing trend in listening frequency.
- **Pricing Strategies**: Offer free trial periods (1-2 months) or reduce premium charges temporarily to encourage more listening.
- **Data-Driven Management**: Utilize exported granular data from the dashboard to present findings to upper management and support informed decision-making.

---

## 🏃 How to Run
1. Clone the repository and download the `.pbix` Power BI file.
2. Open the file in **Power BI Desktop** to view and interact with the visualizations.
3. Use the provided slicers (Platform, Shuffle, Skipped) to dynamically filter the insights.
4. Run the provided `Query_spotify.dax` script in **DAX Studio** to review the underlying calculations.

---

## 🗂️ Repository Structure

```text
├── assets/
│   └── dashboard_preview.png       # Screenshot of the Power BI dashboard
├── data/
│   └── spotify_history.csv         # Raw and pre-cleaned transaction dataset
├── dax/
│   └── Query_spotify.dax           # Analytical queries for KPIs & trend calculations
├── powerbi/
│   └── Spotify_Dashboard.pbix      # Main Power BI file with interactive dashboards
├── docs/
│   ├── Spotify_analysis.docx       # Executive summary and detailed analysis report
│   └── Gamma_Presentation.pdf      # Exported slide deck for stakeholders
└── README.md                       # Project documentation
