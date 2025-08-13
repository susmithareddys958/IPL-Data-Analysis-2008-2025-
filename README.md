# 🏏 IPL Analysis – Power BI Dashboard

This project presents an **interactive Power BI dashboard** that analyzes **Indian Premier League (IPL)** data to uncover insights into **team performance, player achievements, and season trends**.

## 📌 Overview
The dashboard allows users to explore:
- 🏆 **Season Winners & Finalists**
- 📊 **Team Performance** across seasons
- 🏅 **Top Players** (Orange & Purple Cap holders)
- 🎯 **Toss Decision Impact** on match results
- 🏟️ **Venue Analysis** (batting/bowling friendly grounds)

## 🛠️ Tools & Technologies
- **Power BI Desktop** – Data modeling & visualization
- **DAX (Data Analysis Expressions)** – Custom measures & KPIs
- **Data Sources** – IPL matches & deliveries datasets

## 📂 File Information
- **Main File:** `IPL_Analysis(BI).pbix`  
  *(Open with Power BI Desktop)*

## 📊 Key Features
- **Interactive Slicers** for season, team, player, and venue selection
- **Dynamic KPIs** for wins, win percentage, and top performances
- **Custom Visuals** for strike rates, economy rates, and head-to-head records
- **Drill-through Pages** for in-depth player and team stats

## 🧮 Sample DAX Measures
Total Runs = SUM(deliveries[total_runs])

Total Wickets = 
CALCULATE(
    COUNTROWS(deliveries),
    deliveries[is_wicket] = 1
)

Win % = DIVIDE([Wins], [Matches Played], 0)

🚀 How to Use
Clone the repository:
git clone [https://github.com/<your-username>/<your-repo>.git](https://github.com/susmithareddys958/IPL-Data-Analysis-2008-2025-.git)
Open IPL_Analysis(BI).pbix in Power BI Desktop.
