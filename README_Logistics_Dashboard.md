# 🚚 SwiftRoute Logistics Dashboard — Power BI

![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?logo=powerbi&logoColor=black)
![Data Analytics](https://img.shields.io/badge/Analytics-Logistics%20%26%20Operations-0078D4)
![Status](https://img.shields.io/badge/Project-Completed-success)

## 📊 Project Overview

**SwiftRoute Logistics Dashboard** is an interactive Power BI business intelligence project designed to analyze logistics and delivery operations across **orders, drivers, hubs, and vehicles**.

The dashboard transforms operational data into an interactive management reporting solution that helps users monitor:

- Total orders and delivery activity
- On-time delivery performance
- Delayed delivery rate
- Customer satisfaction (CSAT)
- Average delivery time
- Driver performance and experience
- Hub capacity and operational performance
- Vehicle utilization and status
- Vehicle breakdowns and vehicle age
- Monthly and yearly operational trends

The project demonstrates practical skills in **Power BI, DAX, data modeling, KPI development, interactive visualization, drill-down analysis, slicers, and business storytelling**.

---

## 🎯 Business Objective

The primary objective is to provide logistics management with a consolidated view of operational performance and answer questions such as:

1. How many orders are being processed?
2. What percentage of orders are delivered on time?
3. Which drivers have higher or lower delayed-delivery rates?
4. How does driver experience relate to performance ratings?
5. Which hubs handle the highest order volumes?
6. Which hubs have stronger or weaker on-time delivery performance?
7. How does average delivery time vary across hubs and dates?
8. What is the current vehicle fleet status?
9. Which vehicle models contribute to order volume?
10. Which vehicles or vehicle models have higher breakdown levels?
11. How does vehicle age relate to breakdowns?
12. How does customer satisfaction change with operational performance?

---

# 🖥️ Dashboard Pages

The PBIX file contains **four report pages**.

---

## 1. SwiftRoute Logistics Dashboard

The main executive dashboard provides a high-level overview of the logistics operation.

### Key KPIs

- **Total Orders**
- **On-Time Delivery Rate**
- **CSAT %**
- **Average Delivery Time (Hours)**
- **Number of Hubs**
- **Number of Drivers**
- **Number of Vehicles**

### Visual Analysis

The page includes analysis of:

- Vehicle status distribution
- Driver delayed-delivery rate
- Orders by hub
- Hub capacity versus order volume
- Hub on-time delivery rate
- Orders by vehicle model
- Driver experience versus performance rating
- Monthly/yearly filtering

### Business Purpose

This page acts as the **management summary**, allowing users to quickly understand overall logistics performance before moving into driver, hub, or vehicle-level analysis.

---

# 2. 👨‍✈️ Drivers Overview

The Drivers Overview page focuses on workforce performance.

### Key Metrics

- Number of Drivers
- Driver name
- Driver experience / Years of Experience (YOE)
- Performance Rating
- Star Rating
- Delayed Delivery Rate
- Orders handled

### Analysis

The dashboard allows users to investigate:

- Driver-level order performance
- Delayed delivery rates by driver
- Relationship between experience and performance rating
- Driver-specific information
- Monthly and yearly trends
- Total orders over time

### Interactive Features

Users can filter the analysis using:

- Year
- Month
- Driver
- Dynamic measure selection

### Business Questions

This page can help answer:

> Which drivers are associated with higher delivery volumes?

> How does driver experience relate to performance rating?

> Which drivers have higher delayed-delivery rates?

> How does operational workload change over time?

---

# 3. 🏢 Hubs Overview

The Hubs Overview page analyzes logistics hub performance and capacity.

### Key Metrics

- Number of Hubs
- Hub capacity
- Total orders
- On-time delivery rate
- Average delivery time

### Analysis

The page includes:

- Hub capacity versus order volume
- On-time delivery rate by hub
- Daily average delivery time
- Average delivery time by hub
- Date-level operational analysis
- Hub-level performance comparison

### Business Questions

This page can help identify:

- Which hubs process the highest order volumes?
- How does hub capacity compare with order demand?
- Which hubs have higher on-time delivery performance?
- Which hubs have longer average delivery times?
- How does delivery performance change by day?

---

# 4. 🚛 Vehicles Overview

The Vehicles Overview page focuses on fleet performance and reliability.

### Key Metrics

- Number of Vehicles
- Vehicle Status
- Vehicle Model
- Vehicle Code
- Vehicle Age
- Breakdown Count
- Orders handled
- Vehicle Type

### Analysis

The dashboard provides:

- Vehicle status distribution
- Orders by vehicle model
- Vehicle age versus breakdown analysis
- Breakdown count by vehicle code
- Breakdown count by vehicle model
- Orders by vehicle type
- Monthly and yearly filtering

### Business Questions

This page can help investigate:

- How many vehicles are currently available in each status?
- Which vehicle models handle the most orders?
- Which vehicle models have higher breakdown counts?
- Is vehicle age associated with breakdown frequency?
- Which vehicle types contribute most to order volume?

---

# 🧩 Data Model

The Power BI report is structured around logistics operational entities.

### Core Tables / Entities

#### Orders

The order-level data supports analysis of:

- Order volume
- Delivery performance
- Delivery time
- CSAT
- Vehicle type
- Vehicle assignment
- Date-based trends

Important analytical measures include:

- `Total Orders`
- `On Time Delivery Rate`
- `Delayed Delivery Rate`
- `CSAT %`
- `Avg Delivery Time (Hrs)`

#### Drivers

Contains driver-level attributes such as:

- Driver ID / Name
- Experience Years
- Performance Rating
- Star Rating

Used for driver performance and workforce analysis.

#### Hubs

Contains hub-level information including:

- Hub name
- Hub capacity

Used to compare operational capacity with order demand and delivery performance.

#### Vehicles

Contains fleet-level attributes including:

- Vehicle ID
- Vehicle Code
- Vehicle Model
- Vehicle Status
- Vehicle Age
- Breakdown

Used for fleet utilization and reliability analysis.

#### Date Table

A dedicated date dimension supports:

- Year analysis
- Month analysis
- Day-level analysis
- Time-series trends

The report uses date slicers and date-based measures throughout the dashboard.

---

# 📐 Key KPIs

| KPI | Business Purpose |
|---|---|
| **Total Orders** | Measures overall order/delivery volume |
| **On-Time Delivery Rate** | Measures the proportion of deliveries completed on time |
| **Delayed Delivery Rate** | Tracks delivery delays by driver and other dimensions |
| **CSAT %** | Measures customer satisfaction |
| **Avg Delivery Time (Hrs)** | Measures average delivery duration |
| **No. of Drivers** | Measures available driver population |
| **No. of Hubs** | Measures logistics hub coverage |
| **No. of Vehicles** | Measures fleet size |
| **Performance Rating** | Evaluates driver performance |
| **Experience Years** | Provides driver experience context |
| **Hub Capacity** | Measures hub operational capacity |
| **Breakdown** | Measures vehicle reliability issues |
| **Vehicle Age** | Supports fleet-age analysis |

> KPI values are dynamically calculated from the underlying Power BI model and change according to the selected filters.

---

# 🔎 Interactive Dashboard Features

The report includes several interactive Power BI features.

### 📅 Time Filters

Users can filter the report using:

- Year
- Month
- Day-level analysis where available

### 👤 Driver Filters

The Drivers page provides driver-level filtering to investigate individual performance.

### 📊 Dynamic Measure Selection

The report includes a **Select Measure** parameter on the Drivers page, allowing users to dynamically change the analytical measure displayed in the visual.

### 🖱️ Cross-Filtering

Selecting a category in one visual can filter related visuals, enabling interactive exploration of operational performance.

### 📈 Drill-Down / Detailed Analysis

The report supports movement from high-level operational KPIs to detailed:

**Business → Hub → Driver / Vehicle → Operational Metric**

analysis depending on the selected page and visual.

---

# 💡 Business Insights the Dashboard Can Support

The dashboard is designed to uncover operational patterns rather than simply display numbers.

## Delivery Performance

Analyze:

- Overall on-time delivery rate
- Delayed delivery rate by driver
- Average delivery time
- Delivery performance by hub

This can help identify areas where delivery operations may require investigation.

## Driver Performance

Compare:

- Experience years
- Performance rating
- Star rating
- Orders handled
- Delayed delivery rate

This supports workforce-performance analysis.

## Hub Efficiency

Compare:

- Hub capacity
- Order volume
- On-time delivery rate
- Average delivery time

This helps investigate whether differences in hub workload and capacity are associated with delivery outcomes.

## Fleet Reliability

Analyze:

- Vehicle age
- Vehicle model
- Breakdown count
- Vehicle status
- Orders handled

This can help identify fleet-reliability patterns and vehicles that may require operational review.

## Customer Experience

Use:

- CSAT %
- On-time delivery
- Delivery time

to investigate relationships between operational performance and customer satisfaction.

---

# 🛠️ Tools & Technologies

| Technology | Usage |
|---|---|
| **Power BI Desktop** | Dashboard development |
| **Power Query** | Data preparation and transformation |
| **DAX** | Measures, KPIs and analytical calculations |
| **Data Modeling** | Relationships between logistics entities |
| **Power BI Parameters** | Dynamic measure/visual analysis |
| **Interactive Visualizations** | Operational reporting and storytelling |

---

# 🔄 Project Workflow

```text
Raw Logistics Data
        ↓
Data Cleaning & Transformation
        ↓
Data Modeling
        ↓
Relationships
        ↓
DAX Measures & KPIs
        ↓
Interactive Visualizations
        ↓
Dashboard Design
        ↓
Operational Insights
```
---

# 📸 Dashboard Preview

Add screenshots of the four report pages here after exporting them from Power BI:

```markdown
## Dashboard

![SwiftRoute Dashboard](Screenshots/dashboard-overview.png)

## Drivers Analysis

![Drivers Overview](Screenshots/drivers-overview.png)

## Hubs Analysis

![Hubs Overview](Screenshots/hubs-overview.png)

## Vehicles Analysis

![Vehicles Overview](Screenshots/vehicles-overview.png)
```

Adding screenshots is highly recommended because recruiters can understand the project without opening the PBIX file.

---

# 📈 Skills Demonstrated

This project demonstrates practical knowledge of:

- Power BI
- DAX
- Power Query
- Data Modeling
- Data Cleaning
- KPI Development
- Logistics Analytics
- Operations Analytics
- Delivery Performance Analysis
- Driver Performance Analysis
- Hub Performance Analysis
- Fleet Analytics
- Customer Satisfaction Analysis
- Time-Series Analysis
- Interactive Slicers
- Dynamic Parameters
- Cross-Filtering
- Data Visualization
- Business Intelligence
- Data Storytelling

---

# ⭐ Project Highlights

- **4 interactive Power BI report pages**
- Executive logistics dashboard
- Driver performance analysis
- Hub capacity and delivery analysis
- Vehicle fleet analysis
- Total order tracking
- On-time delivery monitoring
- Delayed delivery analysis
- Customer satisfaction monitoring
- Average delivery-time analysis
- Driver experience vs performance analysis
- Vehicle age vs breakdown analysis
- Hub capacity vs order-volume analysis
- Vehicle status analysis
- Dynamic measure selection
- Year and Month filtering
- DAX-based KPIs
- Interactive cross-filtering

---

# ⚠️ Data & Usage Disclaimer

This project is intended for **educational, portfolio, and business-intelligence demonstration purposes**.

The dashboard's conclusions depend on the underlying dataset and selected filters. Operational metrics should be interpreted within the context of the source-data definitions.

If this repository uses a third-party dataset, the original dataset's licensing and usage restrictions continue to apply.

---

# 👨‍💻 Author

**Gaurav Singh**

### Analytics Skills

`Power BI` · `DAX` · `Power Query` · `SQL` · `Excel` · `Tableau`

---

## ⭐ If you find this project useful

Feel free to explore the dashboard, review the data-modeling approach, and use the project as a reference for Power BI logistics and operations analytics.
