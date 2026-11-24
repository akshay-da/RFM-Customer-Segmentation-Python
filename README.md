# RFM Customer Segmentation (Python)

## Overview
RFM analysis (Recency, Frequency, Monetary) to group customers by how recently,
how often, and how much they buy. The project also compares customer spending
by age group and marital status.

## Dataset
- `Customer_Master_Data.csv`: 1,000 customers (age, gender, city, marital status, join date)
- `Customer_Transactions.csv`: 23,050 transactions (customer ID, date, amount)

## Tools Used
- Python, Pandas, NumPy, Matplotlib, Seaborn
- Google Colab (Jupyter Notebook)

## What I Did
- Converted date columns and checked that every transaction matched a customer
- Merged customer and transaction data on CustomerID
- Calculated Recency (days since last purchase), Frequency (number of purchases),
  and Monetary (total spend) for each customer
- Scored each metric from 1 to 5 using business rules and built a 3-digit RFM score
- Assigned customers to segments: Champions, Loyal Customers, Potential Loyalist,
  At Risk, Lost, and Others
- Analyzed segments and spending by age bracket and marital status
- Built bar charts, stacked bar charts, and box plots

## Key Insights
- Loyal Customers are the largest segment: 542 of 1,000 customers (54%)
- 84 customers (8%) are Champions, the best group
- 47 customers (5%) are At Risk and need win-back offers
- Only 2 customers are Lost
- Average spend per customer is close across age groups (about INR 22,700 to 23,300)
- Divorced customers have the highest average spend and Single customers the lowest

## How to Run
1. Download all 3 files into the same place
2. Open `RFM_Analysis.ipynb` in Google Colab
3. Upload the two CSV files to Colab
4. Run all cells

## Future Improvements
- Use quintile-based scoring instead of fixed thresholds
- Add city-wise analysis
- Build a Power BI dashboard from the segments
