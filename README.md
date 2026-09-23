# E-Commerce EDA & Customer Segmentation (RFM) 

This repository contains an exploratory data analysis (EDA) and RFM (Recency, Frequency, Monetary) customer segmentation based on online retail data. The notebook analyzes sales trends, geographic performance, and purchasing behaviors to generate actionable customer segments . 

## Dataset Information
*   **File Used:** `cleaned_online_retail_data_v1.csv` 
*   **Preparation:** The data utilized in this analysis is pre-cleaned. Missing `CustomerID` values were dropped, duplicates were checked, and negative/zero `Quantity` and `UnitPrice` records were removed in a separate preprocessing step (`cleaning.ipynb`) .

## Project Outline
The notebook covers the following analytical phases :
1.  **Data loading & feature engineering:** Extracting `TotalSpend`, `YearMonth`, `Hour`, and `DayOfWeek` .
2.  **Revenue trends over time:** Identifying monthly seasonality .
3.  **Order timing patterns:** Analyzing order volume by hour of day and day of week .
4.  **Geographic revenue breakdown:** Segmenting sales by country .
5.  **Top products:** Identifying best-sellers by quantity sold .
6.  **Customer revenue concentration:** Testing the Pareto (80/20) rule .
7.  **RFM segmentation:** Calculating Recency, Frequency, and Monetary metrics .
8.  **RFM scoring & customer segments:** Assigning scores to group customers .
9.  **Repeat-purchase behavior:** Tracking top customers over time .
10. **Key takeaways:** Final business recommendations .

## Key Business Insights
The exploratory data analysis reveals several critical operational and marketing patterns:

| Focus Area | Key Finding | Actionable Takeaway |
| :--- | :--- | :--- |
| **Seasonality** | November 2011 was the peak month, generating £1.16M in revenue (69% above the monthly average). September and October also showed strong build-up . | Inventory and marketing budgets should be heavily weighted toward the Sep–Nov holiday ramp-up . |
| **Order Timing** | Order volume peaks strictly between 10 AM and 3 PM, hitting its maximum at 12:00 PM (noon) with 3,130 orders. Thursdays are the busiest day, while there is zero order data for Saturdays . | Target time-sensitive marketing promotions and schedule peak customer support staffing for weekday late-mornings . |
| **Geography** | The UK dominates sales, generating ~82% (£7.29M) of total revenue. The Netherlands (£285k) and EIRE (£265k) follow distantly . | The business is highly reliant on the UK market; geographic diversification requires building from a very small base . |
| **Revenue Concentration** | The top 20% of customers (868 out of 4,338) are responsible for 74.7% (£6.63M) of total revenue, closely mirroring the Pareto principle . | Retention efforts and VIP loyalty programs must be laser-focused on this top quintile to protect the core revenue stream . |

## Technologies Used
*   **Python 3**
*   **Pandas & NumPy:** Data manipulation and feature extraction .
*   **Matplotlib & Seaborn:** Data visualization and trend charting .

## How to Run
1. Clone this repository to your local machine.
2. Ensure you have the `cleaned_online_retail_data_v1.csv` dataset in the same directory as the notebook . *(Note: If you only have the raw data, run `cleaning.ipynb` first).*
3. Launch Jupyter Notebook and open the `.ipynb` file to run the cells sequentially.
