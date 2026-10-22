# Nvidia-GPU-Sales-Analytics
Nvidia Sales Dashboard: A C-suite Power BI solution featuring a dark charcoal and neon green theme. Tracks $396M+ revenue, 152K units sold, and GPU performance. Includes interactive slicers for business segments, global regions, and stock status, powered by robust DAX expressions and modern UI/UX design.
# ⚡ NVIDIA Sales Analytics & Executive Intelligence System

An enterprise-grade executive dashboard designed for C-suite decision-makers, built in Microsoft Power BI. This platform transforms complex hardware sales and supply chain data into high-impact operational insights, utilizing a bespoke NVIDIA dark-mode visual hierarchy (`#1A1A1A` Charcoal / `#76B900` Signature Green).

---

## 📈 Executive Summary & Key Highlights
* **Revenue Performance:** Real-time visibility into **$396.06M+** in enterprise revenue across global markets.
* **Volume Tracking:** Monitored delivery and allocation of **152K hardware units**.
* **Segment Intelligence:** In-depth breakdown contrasting high-margin **Data Center AI acceleration** against consumer **Gaming GPU sales**.
* **Market Feedback:** Consolidated pricing indicators (Avg Street Price: **$6.04K**) and customer satisfaction metrics (Avg Rating: **4.43 / 5.00**).

## 🏛️ System Architecture & Visual Design

### 1. C-Suite KPI Performance Strip
* **Top-Level Metrics:** Positioned along the top visual axis for immediate executive assessment.
* **Core KPIs:** Total Revenue, Units Sold, Average Street Price, and Customer Satisfaction Index.

### 2. Strategic Filtering & Control Sidebar
* **Dynamic Slicers:** Native controls allowing instantaneous drill-downs by **Business Segment**, **Geographic Region** (North America, Europe, Asia-Pacific), and **Inventory Status** (`In Stock`, `Low Stock`, `Backordered`).
* **Global Reset:** Single-click canvas restoration for dynamic executive briefings.

### 3. Core Analytical Visualizations
* **Segment Share Analytics:** Donut chart evaluating market contribution between AI enterprise hardware and consumer GPU lines.
* **Geographic Distribution:** Comparative regional bar charts detailing international sales volume and growth.
* **GPU Model Leaderboard:** Clustered ranking isolating top-tier grossing architectures (`B200`, `H100`, `RTX Series`).

---

## 🧮 Explicit DAX Measures & Relational Modeling

The reporting engine leverages explicitly calculated DAX measures to preserve performance and analytical accuracy across variable filter contexts:

```dax
// Total Gross Revenue
Total Revenue = SUM(sales[revenue_usd])

// Total Volume Allocation
Total Units Sold = SUM(sales[units_sold])

// Weighted Average Market Price
Avg Street Price = AVERAGE(sales[avg_street_price_usd])

// Customer Satisfaction Rating
Avg Customer Rating = AVERAGE(sales[customer_satisfaction_score])
