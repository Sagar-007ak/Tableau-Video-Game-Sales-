# Tableau-Video-Game-Sales-
Created an interactive Tableau dashboard to explore global video game sales across genres, platforms, and publishers. Enabled insight-driven analysis through dynamic filters and visualizations like bar charts, tree maps, and bubble charts.

## Table of Contents
- [Introduction](#introduction)
- [Dashboard Requirements](#dashboard-requirements)
- [Installation / Usage](#installation--usage)
- [DAX (Formulas Used in Measures)](#dax-formulas-used-in-measures)
- [Bug / Feature Request](#bug--feature-request)
- [Authors](#authors)

---

## Introduction

This dashboard provides an **interactive analysis of video game sales** across genres, platforms, publishers, and years. It enables users to explore:

- Total sales by genre, platform, and game title  
- Yearly sales trends 
- Top-selling publishers and platforms  
- Filtered insights by region, time, and genre
  
Built using **Tableau**, this project helps identify trends and business patterns in the global video game industry.

---

## Dashboard Requirements

To view and interact with this dashboard, you’ll need:

- **Software:** Tableau Desktop (version 2021.1 or higher recommended)  
- **File:** `Video game sales.twbx` (packaged Tableau workbook)  
- **Dataset Source:** vgsales.csv (from Kaggle or provided source)
- **System Requirements:**
- 4GB+ RAM
- Windows/macOS with Tableau installed  
  
---

## Installation / Usage

1. Open **Tableau Desktop**  
2. Load the `Video game sales.twbx` file  
3. Ensure the data source (`vgsales.csv`) is correctly connected  
   - If needed, replace with your local version of the dataset  
4. Use the dashboard filter controls:
   - **Zone Sales:** NA, EU, JP, Global  
   - **Start Date / End Date:** Filter by year  
   - **Genre:** Filter by game genre  
5. Hover over charts to view **detailed tooltips**  
6. Interact with dashboards and visualizations to explore trends

---

## DAX

- **Calculated Fields and Parameters :**

1. **Zone Sales:** Allows the user to switch between Global, NA, EU, and JP sales zones.
2. **Start Date and End Date:** Used to filter sales by time period.
3. **Genre:** Dropdown parameter to filter data by game genre.
- **Key Calculated Fields:**
4. **Total Sales:** SUM([Global_Sales])
- Calculates the total sales for selected filters.

5. **Top Genres by Sales:** WINDOW_SUM(SUM([Global_Sales]))
- Used to rank genres.
6. **Ranked Titles:** RANK(SUM([Global_Sales]))
- Ranks top 10 games by total sales.
7. **Sales by Year and Genre:**
- Time series calculated by grouping data by Year and Genre fields.

---

## Bug / Feature Request

If you encounter issues or would like to suggest improvements:
- Email: sagar007ak@gmail.com
- Or raise an issue on the project repository (if applicable)

---

## Authors

- **Your Name:** Sagar
- **Role:** Data Analyst / Tableau Developer
- Linkedin: www.linkedin.com/in/sagar1505
- Email: sagar007ak@gmail.com
