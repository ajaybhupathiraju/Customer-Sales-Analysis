Customer-Sales-Analysis

- [Overview](#project-overview)
- [Data Sources](#data-sources)
- [Tools](#tools)
- [Sales Report](#sales-report)
- [Observations](#observations)

 ## Overview
A hardware manufacturing company that produces electronics items. Its products reach end consumers via 3 different channels, like retailers, company-owned retail outlets and a distributor.

We build a [sales report](https://github.com/ajaybhupathiraju/Customer-Sales-Analysis/blob/main/CustomerSales.pdf) that shows countrywide net sales for a customer, and compares last year's sales with current year's sales.   
   
![alt text](/images/CustomerSales.jpg)

 ## Data Sources
[**customer.csv**](data/dim_customer.csv)  
[**countries.csv**](data/dim_market.csv)    
[**products.csv**](data/dim_product.csv)  
[**sales monthly data.csv**](data/fact_sales_monthly.csv)

 ## Tools 
 - csv excel imports
 - Data Cleaning
 - Join tables using Power Query
 - Pivot tables, Power Pivot, DAX functions
 - Conditional formattings.

 ## Sales Report
 1. import data -> from text/csv.
 2. remove duplicate data, replace null values.
 3. Using power query transform data and create a fiscal year "YYYY" to compute net sales.
 4. join tables product_code,customer_code,date and markets.
 5. Using DAX formula create 2019 net sales,2020 net sales and 2021 net sales.
 6. Create a pivot table with country and region as filters, rows -> country and customer
    values -> "2019 net sales","2020 net sales","2021 net sales".
7. apply conditional format.

   [view sales report pdf](https://github.com/ajaybhupathiraju/Customer-Sales-Analysis/blob/main/CustomerSales.pdf)


 ## Observations
1. The top 10 products based on the percentage increase in their net sales from 2020 to 2021 ?
   
 ![alt text](/images/top_10_increase_netsales_2020_2021.jpg)


2. What are the top 5 countries in terms of net sales in 2021?

| Customer        | 2021 NetSales ($ millions) |
| -------------   | -------------              |
| Amazon          | 82.1                       |
| AtliQ Exclusive | 61.1                       |
| AtliQ e Store   | 53.0                       |
| Sage	           | 20.7                       |
| Flipkart        | 19.3                       |

3. What are the new products that began selling in 2021?
   
   | Customer        | 2020 NetSales ($ millions) |2021 NetSales ($ millions) |
   | -------------   | -------------              |-------------              |
   | Nova            |  0                         | 0.4                       |
