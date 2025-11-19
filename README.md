# 📊 Tableau Sales & Financial Dashboard

![Tableau](https://img.shields.io/badge/Tableau-E97627?style=for-the-badge&logo=Tableau&logoColor=white)
![Status](https://img.shields.io/badge/Status-Active-success?style=for-the-badge)

## 📋 Project Overview

An **interactive sales and financial dashboard** built in Tableau, designed for business stakeholders to make data-driven decisions. This dashboard provides comprehensive insights into sales performance, profitability, regional trends, and customer segments through intuitive visualizations and interactive filters.

---

## 🎯 Business Objectives

- Monitor key sales and financial metrics in real-time
- Identify top-performing products, regions, and customer segments
- Analyze sales trends and growth patterns over time
- Enable data-driven decision-making for business stakeholders
- Provide interactive exploration capabilities through filters and drill-downs

---

## 📊 Key Performance Indicators (KPIs)

### Primary Metrics

- **Total Sales Revenue** - Overall sales performance
- **Total Profit** - Profitability measure
- **Profit Margin %** - (Profit/Sales) × 100
- **Order Count** - Total number of transactions
- **Average Order Value** - Sales per order
- **Sales Growth Rate** - Month-over-month/Year-over-year growth

### Secondary Metrics

- Sales by Region (geographic performance)
- Sales by Category & Sub-Category (product analysis)
- Sales by Customer Segment (customer insights)
- Top 10 Products by Sales/Profit
- Shipping Mode Analysis

---

## ✨ Dashboard Features

### a. Interactive Slicers/Filters

- 📅 **Date Range Filter** - Select custom time periods
- 🌍 **Region Filter** - Multi-select geographic regions
- 📦 **Category Filter** - Filter by product categories
- 👥 **Customer Segment Filter** - Consumer, Corporate, Home Office
- 🚚 **Ship Mode Filter** - Delivery method analysis

### b. Time-Series Analysis

- Line charts showing sales and profit trends over time
- Month-over-month and year-over-year comparisons
- Trend lines and forecasting (if applicable)
- Seasonal pattern identification

### c. Summary Cards

- Large KPI cards displaying totals at a glance
- Color-coded indicators (green for positive, red for negative)
- Percentage change indicators
- Dynamic updates based on filter selections

### d. Consistent Color Theme

- **Blue (#1f77b4)** - Sales metrics
- **Orange (#ff7f0e)** - Profit metrics
- **Green (#2ca02c)** - Positive indicators
- **Red (#d62728)** - Negative indicators
- Neutral background for readability

### e. Visual Breakdown Charts

- Bar charts for category/region comparisons
- Geographic map for regional performance
- Pie charts for segment distribution
- Tables for top products ranking

### f. Navigation & Interactivity

- All visuals dynamically respond to filter selections
- Hover tooltips for detailed information
- Click-through drill-down capabilities
- Multiple dashboard pages (if implemented)

---

## 📁 Project Structure

```
Tableau-Sales-Dashboard/
│
├── data/
│   └── superstore_sales.csv          # Source dataset
│
├── dashboards/
│   ├── main_dashboard.twb            # Tableau workbook
│   └── dashboard_packaged.twbx       # Packaged workbook with data
│
├── screenshots/
│   ├── dashboard_overview.png        # Full dashboard view
│   ├── kpi_cards.png                 # KPI metrics display
│   ├── filters_demo.png              # Interactive filters
│   └── time_series_analysis.png      # Trend analysis view
│
├── docs/
│   └── Dashboard_Summary.pptx        # PowerPoint presentation
│
├── README.md                          # Project documentation
└── .gitignore
```

---

## 📦 Dataset Information

**Dataset**: SuperStore Sales Dataset  
**Source**: Kaggle  
**Records**: ~9,000+ transactions  
**Time Period**: 2014-2017 (or your specific period)

### Dataset Fields:

- **Order Information**: Order ID, Order Date, Ship Date, Ship Mode
- **Customer Details**: Customer ID, Customer Name, Segment, Region, State, City
- **Product Information**: Category, Sub-Category, Product Name, Product ID
- **Financial Metrics**: Sales, Quantity, Discount, Profit

---

## 🚀 Getting Started

### Prerequisites

- Tableau Desktop (version 2020.1 or higher)
- SuperStore Sales dataset (included or downloadable from Kaggle)

### Installation & Usage

1. **Clone the repository**
   ```bash
   git clone https://github.com/pshivaprasadreddy/Tableau-Sales-Dashboard.git
   cd Tableau-Sales-Dashboard
   ```

2. **Open in Tableau**
   - Launch Tableau Desktop
   - Open `dashboards/main_dashboard.twb` or `dashboard_packaged.twbx`
   - If using `.twb`, connect to the dataset in `data/` folder

3. **Explore the Dashboard**
   - Use filters to slice data by date, region, category, or segment
   - Hover over visualizations for detailed tooltips
   - Click on elements for drill-down analysis

4. **Customize (Optional)**
   - Modify calculated fields as needed
   - Adjust color themes to match your branding
   - Add additional visualizations or KPIs

---

## 📸 Dashboard Screenshots

### Main Dashboard Overview
![Dashboard Overview](screenshots/dashboard_overview.png)
*Complete dashboard showing KPIs, filters, and key visualizations*

### Time-Series Analysis
![Time Series](screenshots/time_series_analysis.png)
*Monthly sales and profit trends with forecasting*

### Interactive Filters
![Filters](screenshots/filters_demo.png)
*Dynamic filtering capabilities for data exploration*

---

## 💡 Key Insights

Based on the dashboard analysis:

1. **Sales Trends**: Identify growth patterns and seasonal variations
2. **Regional Performance**: Discover top-performing and underperforming regions
3. **Product Analysis**: Determine best-selling categories and profitable products
4. **Customer Segments**: Understand purchasing behavior across different segments
5. **Profitability**: Analyze profit margins and identify optimization opportunities

---

## 🛠️ Technical Implementation

### Tools & Technologies

- **Visualization**: Tableau Desktop
- **Data Source**: CSV (SuperStore Sales Dataset)
- **Calculated Fields**: Profit Margin, AOV, MoM Growth, YoY Growth
- **Features**: Interactive filters, dual-axis charts, maps, KPI cards

### Calculated Fields Created

```tableau
// Profit Margin
SUM([Profit]) / SUM([Sales])

// Average Order Value
SUM([Sales]) / COUNTD([Order ID])

// Month-over-Month Growth
(SUM([Sales]) - LOOKUP(SUM([Sales]), -1)) / ABS(LOOKUP(SUM([Sales]), -1))

// Year-over-Year Growth
(SUM([Sales]) - LOOKUP(SUM([Sales]), -12)) / ABS(LOOKUP(SUM([Sales]), -12))
```

---

## 📚 Learning Outcomes

This project demonstrates:

- Tableau proficiency and dashboard design skills
- Data visualization best practices
- Business intelligence and KPI tracking
- Interactive reporting for stakeholder decision-making

---

## 📝 Future Enhancements

- [ ] Add forecasting models for sales prediction
- [ ] Implement advanced analytics (clustering, outlier detection)
- [ ] Create mobile-responsive dashboard layout
- [ ] Add real-time data refresh capabilities
- [ ] Integrate with additional data sources
- [ ] Develop automated email reports

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/pshivaprasadreddy/Tableau-Sales-Dashboard/issues).

---

## 👨‍💻 Author

**P. Shiva Prasad Reddy**

- GitHub: [@pshivaprasadreddy](https://github.com/pshivaprasadreddy)
- LinkedIn: [P. Shiva Prasad Reddy](https://www.linkedin.com/in/patlolla-shiva-prasad-reddy-2709a4325/)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

## 🎓 Project Context

This dashboard was created as part of a business analytics project to demonstrate:

- Tableau proficiency and dashboard design skills
- Data visualization best practices
- Business intelligence and KPI tracking
- Interactive reporting for stakeholder decision-making

---

## ⭐ Show Your Support

Give a ⭐️ if this project helped you learn Tableau dashboard development!

---

**Last Updated**: November 2025
