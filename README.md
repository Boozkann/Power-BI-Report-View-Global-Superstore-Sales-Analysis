# 📊 Power BI Sales & Customer Analysis Dashboard

## Overview
This Power BI report provides a comprehensive, interactive dashboard for analyzing sales, profit, returns, discounts, shipping, customer segmentation (via RFM), and regional performance. It is structured into modular report pages with dynamic slicers, bookmarks, and role-based access for tailored user experience and data security.

---

## 🗂️ Report Pages & Features

### 1. Overall Performance
**Purpose:** Summarize total business performance.  
**Visuals:**
- KPI Cards: Total Sales, Total Profit, Total Customers, Avg. Delivery Days, Return Rate
- Line Chart: Sales Trend by Order Date  
**Slicers:** Year, Region, Market, Country

---

### 2. Market Sales Trend
**Purpose:** Analyze time-based sales trends.  
**Bookmarks & Visuals:**

#### ➤ Total Sales Trend
- Line Chart by Order Date
- Clustered Column Chart (Monthly/Yearly)
- KPI Cards  
**Slicers:** Year, Segment

#### ➤ Market Sales Trend
- Line Chart (Quarterly Trend)
- KPI Cards  
**Slicers:** Market, Segment, Year

---

### 3. Profit Analysis
**Purpose:** Analyze profit by category, sub-category, and segment.  
**Visuals:** Clustered Bar Chart, Matrix  
**Slicers:** Category, Sub-Category, Market  
**Bookmarks:**
- Total Loss by Category
- Total Net Profit by Category

---

### 4. Discount Analysis
**Purpose:** Analyze how discounts impact profitability.  
**Visuals:** Ribbon Chart  
**Slicers:** Year, Country, Product Category

---

### 5. Regional Analysis
**Purpose:** Explore regional sales volumes and market distribution.  
**Visuals:**
- Map
- Bar Chart (Top/Bottom 5 Countries)
- Donut Chart (Market Share)  
**Slicers:** Country *(limited to Netherlands, India, Turkey, Japan, UK)*  
**Filters:** Top N, Basic Filtering

---

### 6. Category Analysis
**Purpose:** Sales and profit analysis by category and sub-category.  
**Visuals:** Clustered Column Chart, Donut Chart  
**Slicers:** Market  
**Hierarchy:** Segment > Category > Sub-Category  
**Bookmarks:**
- Profit Analysis of Category
- Sales Analysis of Category

---

### 7. Return Analysis
**Purpose:** Analyze return rates and customer behavior.  
**Visuals:**
- Funnel Chart (Customer Count by Segment)
- Table (Top Returned Products/Customers)
- Ribbon Chart (Return Rate Over Time)  
**Slicers:** Market, Year  
**Filters:**
- Return Rate > 15%
- Order Count > 10

---

### 8. Shipping Analysis
**Purpose:** Evaluate delivery performance and costs.  
**Visuals:**
- Bar Charts (Short vs. Long Delivery Durations)
- Column Charts (Ship Mode & Order Priority vs. Delivery Days)
- Line Chart (Shipping Cost Trend)  
**Slicers:** Category, Order Priority, Year  
**Filters:** Top N (Shortest/Longest Deliveries)

---

### 9. RFM Analysis
**Purpose:** Customer segmentation using RFM scoring.  
**Visuals:**
- Bar/TreeMap (Tenure, Recency, Frequency, Monetary, Basket Size)
- Table (Exportable Customer List)
- Matrix (Segment Ratios Across Markets)
- Card (Total & Filtered Customers – with blank protection measure)  
**Slicers:** Tenure, Recency, Frequency, Basket Size  
**Bookmarks:**
- Filter Best Customers: Recency [1–12], Frequency > 4, Basket Size > $500
- Customers at Risk: Recency > 30 months, Frequency [4–8]
- Champions of Corporate: Recency Score = 5, Frequency Score = 5, Monetary > $1000  
**Extras:**
- “Clear All Slicers” Button
- Customized slicer-to-chart interactions

---

### 10. Main Page (Home)
**Purpose:** Navigation hub.  
**Features:**
- Quick-access buttons to all report pages and bookmarks
- “Back” buttons for seamless navigation

---

### 11. Row-Level Security (RLS)
**Purpose:** Enforce access control based on user roles.  
**Defined Roles:**
- **Regional Role:** Users can view only data from their assigned region (e.g., APAC).
- **Segment Role:** Marketing users see only “at-risk” customer segments.
- **Country-Based Role:** Users have access limited to specific countries (e.g., Netherlands only).

---

## 🔧 Tools & Technologies
- Power BI Desktop (Optimized for latest version)
- DAX Measures & Calculated Columns
- Bookmarks, Buttons, Navigation Actions
- Row-Level Security (RLS)
- Export-friendly visuals (tables, matrices)

