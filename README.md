SWYNEX Exploratory Data Analysis

Task 2 — Exploratory Data Analysis

This project performs Exploratory Data Analysis (EDA) on a cleaned Online Retail dataset using Python, Pandas, NumPy, Matplotlib, and Seaborn.

The analysis goes beyond basic statistics and explores revenue trends, customer behavior, product performance, geographic distribution, customer revenue concentration, RFM segmentation, and repeat-purchase behavior.

Project Objectives

Explore the cleaned retail dataset

Identify revenue trends over time

Analyze order timing by hour and day of week

Compare revenue across countries

Identify the most-sold products

Analyze customer revenue concentration using the Pareto principle

Build RFM (Recency, Frequency, Monetary) customer segments

Analyze repeat-purchase behavior among the highest-spending customers

Extract useful business insights from the data

Technologies Used

Python

Pandas

NumPy

Matplotlib

Seaborn

Jupyter Notebook

Project Structure

SWYNEX-Exploratory-Data-Analysis/
│
├── EDA_clean.ipynb
├── cleaned_online_retail_data_v1.csv
└── README.md

cleaned_online_retail_data_v1.csv is the cleaned dataset produced in Task 1 and is required to run the notebook.

Analysis Sections

1. Setup & Data Loading

Loads the cleaned dataset and prepares the Python libraries used for analysis.

2. Feature Engineering

Creates analysis-ready features including:

TotalSpend

YearMonth

Hour

DayOfWeek

3. Revenue Trends Over Time

Calculates monthly revenue and visualizes changes over time.

4. Order Timing Patterns

Analyzes the number of unique orders by:

Hour of day

Day of week

5. Geographic Revenue Breakdown

Ranks countries according to total revenue and visualizes the top countries.

6. Top Products

Identifies the products with the highest total quantity sold.

7. Customer Revenue Concentration

Uses cumulative customer spending to investigate how revenue is distributed across customers.

8. RFM Segmentation

Calculates:

Recency: days since the customer's last purchase

Frequency: number of distinct orders

Monetary: total amount spent

9. RFM Scoring & Customer Segments

Converts RFM values into 1–5 scores and assigns customers to segments such as:

Champions

Loyal Customers

New Customers

Promising

At Risk

Needs Attention

Hibernating / Lost

10. Repeat-Purchase Behavior

Focuses on the highest-spending 20% of customers and measures purchase frequency and average time between purchases.

Key Findings

The notebook produced the following results from the analyzed dataset:

Dataset size: 392,692 cleaned transaction records were analyzed, representing 4,338 customers.

Revenue by month: November 2011 generated the highest monthly revenue at approximately £1.156M.

Order timing: The highest number of unique orders occurred at 12:00, with 3,130 orders. By day of week, Thursday recorded the highest number with 4,032 orders.

Geographic concentration: The United Kingdom generated approximately £7.285M in revenue, substantially more than the other countries in the dataset.

Top-selling product: PAPER CRAFT , LITTLE BIRDIE recorded the highest total quantity sold, with 80,995 units.

Customer revenue concentration: The top 20% of customers (868 customers) generated approximately 74.7% of total revenue.

RFM segmentation: The Champions segment contained 1,121 customers and accounted for approximately 65.9% of total revenue.

Repeat purchasing: Among the top 20% highest-spending customers, the median interval between purchases was approximately 33.8 days.

Business Interpretation

The analysis shows that revenue is highly concentrated among a relatively small group of customers, while customer behavior varies considerably across RFM segments.

The analysis also identifies clear patterns in purchasing time, geography, products, and repeat-purchase behavior. These patterns can be used as a basis for further customer analysis and business decision-making.

How to Run

Clone the repository:

git clone https://github.com/YOUR_USERNAME/SWYNEX-Exploratory-Data-Analysis.git

Open the project:

cd SWYNEX-Exploratory-Data-Analysis

Make sure the following files are in the same folder:

EDA_clean.ipynb
cleaned_online_retail_data_v1.csv

Launch Jupyter Notebook:

jupyter notebook

Open EDA_clean.ipynb and run the cells.

Task Submission

This repository was created as part of SWYNEX Technologies Internship — Task 2: Exploratory Data Analysis.




Author

Mohamed Ben Abbes

Data Analysis / IT Background
