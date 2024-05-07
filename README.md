Customer-Sales-Analysis

- [Overview](#overview)
- [Data Sources](#data-sources)
- [Tools](#tools)
- [Sales Report](#sales-report)
- [Observations](#observations)

 ## Overview
A hardware manufacturing company that produces electronics items. Its products reach end consumers via 3 different channels, like retailers, company-owned retail outlets and a distributor.

We build a [sales report](https://github.com/ajaybhupathiraju/Customer-Sales-Analysis/blob/main/CustomerSales.pdf) that shows countrywide net sales for a customer, and compares last year's sales with current year's sales, compute % of revenus increase and top n countries in sales growth etc.  
   
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
 1. Import data -> from text/csv.
 2. Remove duplicates, replace null values in data.
 3. Using power query transform data and create a fiscal year "YYYY" to compute net sales.
 4. Join tables product_code,customer_code,date and markets.
 5. Using DAX formula created "2019 net sales","2020 net sales" and "2021 net sales".
 6. Create a pivot table with country and region as filters
    rows -> country and customer
    values -> "2019 net sales","2020 net sales","2021 net sales" and "2020 vs 2021".
8. apply conditional format.

   [view sales report pdf](https://github.com/ajaybhupathiraju/Customer-Sales-Analysis/blob/main/CustomerSales.pdf)


 ## Observations
 
1. The top 10 customers based on the percentage increase in their net sales from 2020 to 2021 ?
   
 ![alt text](/images/Top10_Netsales_increased_2020_21.jpg)


2. What are the top 5 customers in terms of net sales in 2021?

   | Customer        | 2021 NetSales (in millions)|
   | -------------   | -------------              |
   | Amazon          | 82.1                       |
   | AtliQ Exclusive | 61.1                       |
   | AtliQ e Store   | 53.0                       |
   | Sage	           | 20.7                       |
   | Flipkart        | 19.3                       |

3. What are the new products that AtliQ began selling in 2021?
   
   | Customer        | 2020 NetSales (in millions) |2021 NetSales (in millions) |
   | -------------   | -------------               |-------------               |
   | Nova            |  0                          | 0.4                        |

4. What are the top 5 countries in terms of net sales in 2021?

   | Country         | 2021 NetSales (in millions)|
   | -------------   | -------------              |
   | India           | 161.3                      |
   | USA             | 87.8                       |
   | South Korea     | 49.0                       |
   | Canada          | 35.1                       |
   | United Kingdom  | 34.2                       |
   
