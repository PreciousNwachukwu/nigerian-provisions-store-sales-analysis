# Nigerian Provisions Store — Vendor Sales Analysis
 
**Tool:** Python (pandas, numpy, matplotlib)  
**Dataset:** 500 simulated sales transactions | Jan – Dec 2024  
**Context:** General provisions store, Abuja, Nigeria  
**Author:** Precious Nwachukwu | Data Analyst
 
---
 
## Project Overview
 
This project analyses a full year of sales data from a Nigerian general provisions store, the kind of neighbourhood shop that stocks everything from Dangote Rice and Indomie noodles to Milo, palm oil, and Pampers.
 
The goal was to answer practical business questions that matter to a small retail owner: which products and categories drive the most revenue, when sales peak, how discounting affects profitability, and what payment methods customers prefer.
 
The dataset was simulated using realistic Nigerian product names, Naira pricing, and demand logic that reflects actual consumer behaviour, including festive season surges in November and December, higher weekend footfall, and end-of-month salary spending patterns.
 
---
 
## Business Questions
 
1. Which product categories generate the most revenue and profit?
2. What are the top-performing individual products?
3. How does sales performance vary by month and day of week?
4. Which payment methods do customers prefer?
5. What is the impact of discounting on profit margins?
---
 
## Dataset Structure
 
| Column | Description |
|---|---|
| transaction_id | Unique transaction reference (TXN1000+) |
| date | Transaction date (2024-01-01 to 2024-12-31) |
| month | Month name |
| day_of_week | Day of the week |
| product_name | Product name (e.g. Indomie Noodles, Dangote Rice) |
| category | Product category (6 categories) |
| quantity_sold | Units sold per transaction |
| unit_cost_ngn | Cost price per unit (NGN) |
| unit_price_ngn | Selling price per unit (NGN) |
| discount_pct | Discount applied: 0%, 5%, or 10% |
| total_revenue_ngn | Total revenue for the transaction |
| total_cost_ngn | Total cost for the transaction |
| profit_ngn | Profit = Revenue minus Cost |
| profit_margin_pct | Profit margin as a percentage |
| payment_method | Cash, Transfer, or POS |
 
**Product categories covered:** Grains & Staples, Beverages, Oils & Condiments, Personal Care, Household & Cleaning, Snacks & Confectionery
 
---
 
## Key Findings
 
### Revenue & Category Performance
- **Beverages** was the top revenue-generating category at **N1.47 million** for the year
- **Grains & Staples** came second at **N1.15 million**, driven by consistent demand for rice, garri, and noodles
- **Snacks & Confectionery** had the highest average profit margin at **23.0%**, despite being the third-lowest revenue category making it the most efficient category by profitability
### Top Products
- **Eva Water 75cl x12** was the single highest-revenue product at **N227,900**
- **Lacasera Apple Drink x6** and **Mama Gold Rice 5kg** followed closely at **N184,000** each
- Fast-moving consumer goods (Indomie, Maggi Cubes, Gala Sausage Roll) consistently appeared in the top transaction volume rankings
### Seasonal Trends
- **December** was the peak month with **N668,160** in revenue, a clear festive season effect
- **January and February** were the weakest months, consistent with post-festive consumer pullback
- May showed a mid-year spike, likely driven by end-of-school-term household stocking
### Day of Week Patterns
- **Saturday** generated the highest daily revenue
- **Wednesday and Thursday** had the most transactions by volume, suggesting regular mid-week restocking behaviour
- **Monday** was consistently the slowest day for both revenue and transactions
### Payment Methods
- **Cash** dominated at **54.8%** of all transactions
- **Bank Transfer** accounted for **30.4%**, reflecting growing mobile banking adoption in Nigeria
- **POS** accounted for the remaining **14.8%**
### Discount Impact
- Transactions with **0% discount** averaged a **20.7% profit margin**
- **5% discounts** reduced margins to **16.2%**
- **10% discounts** cut margins further to **11.6%**, nearly halving profitability compared to full-price sales
---
 
## Recommendations
 
1. **Stock up Beverages and Grains in October–December.** The festive season consistently drives around 50% more demand, running out of stock during this period is a direct revenue loss.
2. **Limit 10% discount events.** A 10% discount reduces average margins by nearly 9 percentage points compared to full-price sales. If discounts are used, 5% is a safer threshold that still incentivises purchases without severely impacting profitability.
3. **Promote POS and bank transfer payments.** With 54% of transactions still in cash, there is meaningful operational risk in cash handling and reconciliation. Incentivising digital payments even slightly would reduce this risk.
4. **Maintain buffer stock for fast movers on Fridays and Saturdays.** Products like Indomie, Maggi Cubes, and Gala Sausage Roll see their highest demand at weekends. Stockouts on these days disproportionately affect revenue.
5. **Review Snacks & Confectionery pricing strategy.** At 23% average margin, the highest of all categories. This category is underweighted in the product mix. Expanding variety or shelf space here could improve overall store profitability without increasing operational complexity.
---
 
## Tools & Libraries
 
```python
pandas       # Data manipulation and aggregation
numpy        # Numerical operations and random simulation
matplotlib   # Data visualisation (bar charts, line charts, pie charts)
datetime     # Date generation and time-series logic
```
 
---
 
## Charts Produced
 
| Chart | Description |
|---|---|
| Category Revenue & Margin | Side-by-side horizontal bar charts comparing revenue and profit margin by category |
| Top 10 Products | Horizontal bar chart of highest-revenue individual products |
| Monthly Trend | Line chart showing revenue and profit across all 12 months with peak annotation |
| Day of Week | Dual bar charts showing revenue and transaction count by weekday |
| Payment Methods | Dual pie charts by transaction count and revenue value |
| Discount Impact | Bar chart showing how 0%, 5%, and 10% discounts affect average profit margin |
 
---
 
## How to Run
 
1. Open [Google Colab](https://colab.research.google.com)
2. Create a new notebook
3. Copy cells from `vendor_analysis_COLAB_CELLS.py` in order
4. Run all cells, the dataset is generated programmatically, no file upload needed
---
 
## Author
 
**Precious Nwachukwu**  
Data Analyst | GIS Analyst | Abuja, Nigeria  
[LinkedIn](https://linkedin.com/in/precious-nwachukwu-873b432b7) | [Portfolio
