# CRM Sales Opportunities Analytics

**Comprehensive exploratory and predictive analytics on a B2B sales pipeline with dynamic reporting and visualizations.**

A Python-based project analyzing 8,800+ opportunities across 85 accounts to uncover insights about sales performance, pipeline health, revenue drivers, and strategic growth opportunities.

---

## 🎯 Project Overview

This project demonstrates end-to-end **data analytics and business intelligence** work on a realistic B2B CRM dataset. The analysis combines data cleaning, exploratory data analysis (EDA), advanced segmentation (RFM), win/loss analytics, pipeline velocity modeling, and dynamic Matplotlib/Seaborn dashboards—all reproducible in a Google Colab notebook.

### Key Highlights

- **8,800 opportunities** across 35 sales agents, 85 accounts, and 7 products
- **$10.0M in won revenue** with a 48.2% global conversion rate
- **51.8-day average sales cycle** with monthly revenue ranging $0.7M–$1.3M
- **4 executive dashboards** with win rates, trends, performer rankings, and pipeline health metrics
- **9 detailed analysis exports** (CSV) for further stakeholder use

---

## 📊 Key Results

### Pipeline & Revenue

- **Stage distribution:** 48% Won, 28% Lost, 18% Engaging, 6% Prospecting (thin forward pipeline at 0.5x coverage)
- **Monthly revenue volatility:** $0.7M–$1.3M, indicating strong seasonality
- **Pipeline velocity:** $45.8K/day → projected $1.37M (30 days) and $4.12M (90 days)
- **Win/Loss ratio:** 1.71:1, showing healthy close rates relative to losses

### Top Performers

- **Best agent:** Darcel Schlecht ($1.15M revenue, 349 deals won, $3.3K avg deal size)
- **Most efficient agent:** Reed Clapper ($1.85K revenue per opportunity, 65.4% conversion)
- **Top product:** GTXPro ($3.51M revenue, 729 units sold)
- **Top region:** West ($3.57M revenue, 63.9% win rate)

### Customer Segments & Sectors

- **RFM Champions:** 24 accounts generating $3.89M (38.9% of total)
- **At-Risk accounts:** 9 accounts with $0.74M historical revenue—high recovery potential
- **Top sector:** Retail ($1.87M), followed by Technology and Medical
- **Company size impact:** Enterprise accounts average $156K per account; strongest win rates across all sizes

### Conversion & Win Rates

- **Regional win rates:** 62.6% (Central) to 63.9% (West)—consistent performance
- **Best products:** MG Special and GTX Plus Pro (~64% win rates)
- **Price dynamics:** Low (<$1K) and High (>$5K) products both achieve ~64% win rates; mid-range lags at 61%
- **Top manager:** Cara Losch (64.4% win rate, 480 deals won)

---

## 📁 Dataset

The analysis uses four CSV files representing a complete B2B CRM system:

- **sales_pipeline.csv** – Opportunities (ID, agent, product, account, stage, engagement date, close date, close value)
- **accounts.csv** – Account metadata (name, sector, revenue, employee count, parent company)
- **sales_teams.csv** – Sales organization (agent, manager, regional office)
- **products.csv** – Product catalog (name, series, list price)

All data is synthetic and designed for educational and portfolio purposes.

---

## 🔧 Features & Analysis Blocks

### 1. Sales Pipeline EDA
- Stage distribution and conversion rates
- Revenue by pipeline stage
- Time-to-close metrics and monthly revenue trends
- Pipeline velocity and 90-day forecasts

### 2. Performance Analytics
- Top agents, products, sectors, and regions by revenue and win rate
- Manager-level KPIs and revenue per agent
- Efficiency metrics (revenue per opportunity)

### 3. Advanced CRM Analytics
- RFM (Recency, Frequency, Monetary) segmentation with account health classification
- Win/loss breakdown by region, product series, manager, and price band
- Account size analysis (Small, Medium, Large, Enterprise)
- Subsidiary vs. independent company performance

### 4. Predictive Analysis
- Close probability by region, product series, sector, manager, and price category
- Deal-size impact on conversion and sales cycle
- Combination analysis (e.g., region × product, manager × product)

### 5. Dynamic Dashboard & Reporting
- **CRMAnalytics class** that:
  - Dynamically computes KPIs from raw data
  - Generates 4 professional PNG dashboards (pipeline overview, top performers, trends, pipeline health)
  - Creates formatted text executive summary
  - Exports 9 CSV files for downstream analysis

---

## 🚀 Tech Stack

- **Python 3.x**
  - **Pandas** – Data manipulation and groupby analysis
  - **NumPy** – Numerical computations
  - **Matplotlib & Seaborn** – Data visualization and charting
- **Google Colab** / Jupyter Notebook
- **CSV** – Data storage

---

## 📖 Getting Started

### Option 1: Open in Google Colab (Recommended)

1. Clone or download this repository
2. Upload `CRM Sales Opportunities.ipynb` and all CSV files to Google Drive
3. Open the notebook in Colab
4. Run cells in sequence—all outputs (CSVs and PNG charts) will be saved to your Colab environment

### Option 2: Run Locally

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/crm-sales-analytics.git
   cd crm-sales-analytics
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Place CSV data files in the `data/` directory

4. Run the notebook in Jupyter:
   ```bash
   jupyter notebook "CRM Sales Opportunities.ipynb"
   ```

---

## 📤 Outputs

### CSV Reports (9 files)
- `agent_performance.csv` – Agent revenue, deals won, avg deal size
- `agent_conversion_analysis.csv` – Win rates, efficiency, revenue per opportunity
- `product_performance.csv` – Product revenue, units sold, profitability
- `sector_analysis.csv` – Revenue by industry vertical
- `regional_performance.csv` – Regional office metrics
- `manager_performance.csv` – Manager KPIs and team revenue
- `account_detailed_analysis.csv` – Account-level performance with company size
- `deals_enhanced_analysis.csv` – Deal-level features (region, series, sector, price)
- `pipeline_velocity_by_agent.csv` – Agent velocity with 30-day projections
- `customer_segmentation_rfm.csv` – RFM segments and account health classification

### PNG Dashboards (4 files)
- **crm_pipeline_overview.png** – Stage distribution, revenue by stage, win/loss ratio
- **crm_top_performers.png** – Top 10 agents by revenue, top 7 products, revenue by region, top 10 agents by conversion
- **crm_trends_analysis.png** – Monthly revenue, deals closed, avg deal size, sales cycle over time
- **crm_pipeline_health.png** – Sales funnel, win rate by sector, deal size distribution, sales cycle distribution

---

## 💡 How to Use This Project

### For Portfolio Building
Showcase your ability to:
- Clean and prepare real-world data
- Perform advanced segmentation (RFM) and multi-dimensional analysis
- Build reusable, object-oriented Python classes
- Create professional visualizations for stakeholders
- Translate data insights into actionable business recommendations

### As a Template
Adapt this project for:
- Internal CRM analytics projects
- Sales forecasting and pipeline management
- Customer segmentation and retention strategies
- Performance benchmarking and territory analysis

### For Learning
Study:
- Pandas groupby, aggregation, and merge patterns
- Data visualization best practices (Matplotlib/Seaborn)
- Class design for analytics workflows
- Business metrics and KPI definitions

---

## 📊 Repository Structure

```
.
├── CRM Sales Opportunities.ipynb    # Main notebook (all analysis and charts)
├── data/
│   ├── sales_pipeline.csv
│   ├── accounts.csv
│   ├── sales_teams.csv
│   └── products.csv
├── outputs/
│   ├── *.csv                        # Exported analysis files
│   └── *.png                        # Dashboard visualizations
├── requirements.txt
└── README.md
```

---

## 🎓 Key Insights & Recommendations

### Immediate Priorities (Next 30 Days)
1. **Champion account management** – Dedicate resources to 24 Champions accounts generating $3.89M
2. **At-risk recovery** – Reactivate 9 at-risk accounts with $0.74M recovery potential
3. **Conversion optimization** – Roll out West region best practices (63.9% win rate) across all regions
4. **Risk diversification** – Expand into underserved sectors (employment, services, telecom) to reduce top-10 concentration from 21% to <15%

### Growth Levers
- **Pipeline coverage:** Currently at 0.5x; target 3x via prospecting volume increase → potential +200% revenue
- **Sales cycle reduction:** Lower from 52 to 45 days = +15% annual throughput
- **Product mix optimization:** Mid-price products lag slightly in win rate; consider bundling with high-margin low-price SKUs
- **Price testing:** Low and high-price products perform equally well; test premium positioning for enterprise accounts

---

## 🔗 Connect

Questions, feedback, or collaboration opportunities? Reach out on **LinkedIn: [carlscamt](https://www.linkedin.com/in/carlscamt)**

---

## 📝 License

This project is provided as-is for educational and portfolio purposes. Feel free to adapt and use as a template for your own analytics work.

---

## 🙏 Acknowledgements

- CRM and sales pipeline analytics best practices
- Data visualization design principles (Matplotlib, Seaborn)
- GitHub README structure and templates
