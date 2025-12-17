# Mobile Sales Dashboard — Power BI

An interactive **Power BI** dashboard that visualizes a synthetic mobile sales dataset.
This was my **first dashboard in Power BI** — I built it to learn the end-to-end flow: generate data, clean it, model it, and design an interactive, easy-to-read dashboard.

---

## What this dashboard does

The dashboard helps you explore mobile sales patterns and surface quick insights:

* **Top summary KPIs:** Total sales, total quantity, total transactions (snapshot).
* **Time trends:** Monthly sales/quantity trend and year-over-year comparisons.
* **Day-wise performance:** Sales by day name to spot which weekdays perform best/worst.
* **Geography:** City-wise sales plotted on a map.
* **Top products:** Top-selling mobile models.
* **Customer ratings:** Rating distribution and counts.
* **Transactions breakdown:** Payment method split (UPI, Debit/Credit Card, Cash).
* **Interactive filters:** Brand, Mobile Model, Day Name, Payment Method for fast exploration.

> Example : **769M** total sales · **19K** total quantity · **4K** total transactions.

---

## How I built it

* **Data generation:** I generated a dummy mobile sales dataset using **ChatGPT** (to simulate realistic sales records).
* **Data cleaning & transformation:** Used **Power Query** inside Power BI Desktop to load and transform the raw data (rename columns, data types, date parsing, calculate helper columns).
* **Modeling & measures:** Created basic DAX measures for totals, trends, and percentages to drive the visuals.
* **Visuals & layout:** Built interactive visuals (map, line charts, area chart, bar charts, pie chart) and focused on a clean layout and balanced color palette for readability and presentation.
* **Interactivity:** Added slicers and cross-filtering so every visual is interactive.

---

## Features / Visuals

* KPI cards (Total Sales, Total Quantity, Transactions)
* Line/area charts for monthly and day-wise trends
* Filled map for city-wise sales distribution
* Horizontal bars for top mobile models
* Funnel / bar for customer ratings
* Pie chart for payment method distribution
* Filter pane with Brand, Mobile Model, Day Name, Payment Method

---

## Repository structure

```
/Icons/
│  ├─ Logo.png                     → Dashboard header/logo icon
│  ├─ Total sales img.png          → KPI icon for Total Sales
│  ├─ Total Quantity img.png       → KPI icon for Total Quantity
│  └─ Total Transactions img.png   → KPI icon for Total Transactions

Dashboard.pbix                     → Main Power BI report file
Mobile Sales Data.xlsx             → Source dataset used in the dashboard
Dashboard img.png                  → Screenshot of the final dashboard
README.md                          → This file

```
Dashboard.pbix contains Power Query transformations, DAX measures, visuals, and interactions.

Mobile Sales Data.xlsx is the raw dataset connected to the report.

Icons are stored separately to keep the project organized and reusable.

Dashboard img.png allows viewers to preview the dashboard without opening Power BI.
---

## How to open & explore

1. Download the `Dashboard.pbix` file and open it in **Power BI Desktop (recommended desktop version)**.
2. The report contains Power Query transformations and a saved data snapshot, so you can explore visuals without the original data if needed.
3. To refresh with the included sample CSV:

   * In Power BI Desktop: **Home → Transform data → Data source settings** (update path) or open Power Query Editor and edit the Source step.
   * Then click **Refresh** (or **Refresh All**) in Power BI Desktop.
4. If you want to regenerate the dummy dataset, use the `data/README` (or a simple script) — the repo includes the sample CSV so you can reproduce visuals right away.

---

## Tips & notes

* The PBIX stores a snapshot (pivot/cached data). If you move the file to a different machine, update the Power Query Source paths before refreshing.
* Map visuals may require an internet connection for map tiles.
* If you share the PBIX, either bundle the sample CSV in `/data/` or keep queries pointing to relative paths/parameters so others can refresh easily.

---

## Why I made this

This project helped me practice:

* Data generation & thinking about realistic fields for sales data
* Power Query transformations and handling messy data
* DAX basics for KPIs and trend measures
* Visual design principles: spacing, color palette, and readable KPIs
  It was a great hands-on way to learn the Power BI workflow.

---

## Demo

▶️ Watch the screen recording demo:
👉 

---

## License & reuse

Feel free to reuse or adapt this dashboard for learning or demos. If you republish or fork, a small attribution is appreciated.

---

## Contact

If you’d like to discuss improvements, feedback, or collaboration — connect with me:
- LinkedIn: [Ashutosh Kumar Jalan](https://www.linkedin.com/in/ashutoshjalan-/)


---
