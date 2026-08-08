# 🚛 America Truck Business Analysis — Power BI Dashboard

An interactive business analysis dashboard built in Power BI. The project analyzes U.S. trucking business data and uses DAX to build year-over-year comparative metrics.

## 📌 About the Project

The dataset was provided as a prepared Excel file and loaded into Power BI, where it was modeled using a star schema. The goal was to build a dashboard that tracks key business metrics — revenue, profit, and delivery efficiency — in real time and compares them against the previous year.

## 🛠 Tools Used

- **Power BI Desktop** — data modeling and visualization
- **DAX** — measures and time intelligence
- **Excel** — source data

## 🗂 Data Model

Star schema architecture:
- **Trip** — fact table (per-trip data: revenue, cost, distance, date, etc.)
- **State** — dimension table for geographic breakdown by state

## 📐 DAX Measures

- Total Revenue and Profit
- Delivery Rate
- Active driver and truck counts
- Year-over-year comparison using `SAMEPERIODLASTYEAR` / `DATEADD` functions
- Conditional ▲ / ▼ trend indicators with color formatting (green for growth, red for decline)

## 📊 Dashboard Features

- KPI cards showing key metrics and their year-over-year trend
- Gauge visual for tracking targets vs. actuals
- Line charts for time-based trend analysis
- Clustered bar chart and table for state-level comparison
- Slicers for filtering by date, state, and other dimensions
- Dark and Light mode, built as separate report pages

## 🔍 Key Insights & Recommendations

A few things stood out while analyzing the data.

Profit margin slipped slightly (from ~52% to ~50%) even though revenue stayed stable — a sign that costs are rising faster than revenue, worth a closer look.

One driver has a noticeably lower delivery success rate (~84% vs. ~91% average), and a large share of failed deliveries trace back to them — likely worth investigating the cause.

A few trucks and specific long-haul routes consistently show lower margins than the rest of the fleet, suggesting they could use a maintenance check or a pricing review.

Overall, the dashboard is most useful when checked regularly to catch under performing drivers, trucks, and routes early.


## 🖼 Screenshots

> Screenshots of the dashboard pages are in the `screenshots/` folder.

## 🚀 How to Open

1. Install [Power BI Desktop](https://www.microsoft.com/power-platform/products/power-bi/downloads)
2. Download the `.pbix` file
3. Open it with Power BI Desktop

## 📫 Contact

Feel free to reach out via LinkedIn with any questions or feedback.
