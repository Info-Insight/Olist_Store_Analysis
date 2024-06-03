**Sales Analysis of Olist E-commerce Store**

**Introduction**


The Olist sales dataset is a collection of anonymized data about orders placed on the Olist from September 2016 to September 2018. It contains a wide range of information about each order, including the order date, product details, payment and shipping information, customer and seller IDs, and customer reviews. The dataset also includes information about the sellers who list their products on Olist, as well as data on customer behavior and demographics. The dataset is designed to help analysts and researchers better understand the e-commerce landscape in Brazil and identify opportunities for growth and optimization.

**Power BI Skills/Concepts applied:**

1) Data Cleaning/Validation in Power Query
2) Data Modelling
3) Data Visualization
4) DAX Concepts: Calculated Measures, Calculated Columns.
5) Filters and slicers

**About the Data**


The raw data was gotten from https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce. It contains 9 tables which are Olist_customers, Olist_geolocation, Olist_order_items, Olist_order_payments, Olist_order_reviews, Olist_orders, Olist_products, Olist_sellers, Product_category_name.

**Data Dictionary**


**1) olist_customers_dataset.csv**


customer_id: unique identifier for each customer

customer_unique_id: unique identifier for each customer (anonymized)

customer_zip_code_prefix: zip code prefix of the customer's address

customer_city: city where the customer is located

customer_state: state where the customer is located

**2)	olist_geolocation_dataset.csv**


geolocation_zip_code_prefix: zip code prefix for the location

geolocation_lat: latitude of the location

geolocation_lng: longitude of the location

geolocation_city: city of the location

geolocation_state: state of the location


**3)	olist_orders_dataset.csv**

order_id: unique identifier for each order

customer_id: unique identifier for the customer who placed the order.

order_status: current status of the order (e.g. delivered, shipped, canceled)

order_purchase_timestamp: date and time when the order was placed

order_approved_at: date and time when the payment for the order was approved

order_delivered_carrier_date: date and time when the order was handed over to the carrier

order_delivered_customer_date: date and time when the order was delivered to the customer

order_estimated_delivery_date: estimated date when the order is expected to be delivered


**4)	olist_order_items_dataset.csv**

order_id: unique identifier for the order

order_item_id: unique identifier for each item within an order

product_id: unique identifier for the product being ordered

seller_id: unique identifier for the seller who listed the

product shipping_limit_date: date and time when the seller has to ship the product

price: price of the product

freight_value: shipping fee for the product


**5)	olist_order_payments_dataset.csv**

order_id: unique identifier for the order

payment_sequential: index number for each payment made for an order

payment_type: type of payment used for the order (e.g. credit card, debit card, voucher)

payment_installments: number of installments in which the payment was made

payment_value: value of the payment made
**6)	olist_products_dataset.csv**

product_id: unique identifier for each product

product_category_name: name of the category that the product belongs to

product_name_lenght: number of characters in the product name

product_description_lenght: number of characters in the product description

product_photos_qty: number of photos for the product

product_weight_g: weight of the product in grams

product_length_cm: length of the product in centimeters

product_height_cm: height of the product in centimeters

product_width_cm: width of the product in centimeters

**7)	olist_sellers_dataset.csv**

seller_id: unique identifier for each seller

seller_zip_code_prefix: zip code prefix for the seller's location

seller_city: city where the seller is located

seller_state: state where the seller is located

**8)	product_category_name_translation.csv**

product_category_name: name of the product category in Portuguese

product_category_name_english: name of the product category in English

**9)	olist_order_reviews_dataset.csv**
review_id: unique identifier for each review

order_id: unique identifier for the order that the review is associated with

review_score: numerical score (1-5) given by the customer for the product

review_comment_title: title of the review comment

review_comment_message: text of the review comment

review_creation_date: date and time when the review was created

review_answer_timestamp: date and time when the seller responded to the review

**Business Question**
1) What is the total revenue generated by Olist, and how has it changed over time?
2) How many orders were placed on Olist, and how does this vary by month or season?
3) What are the most popular product categories on Olist, and how do their sales volumes.
4) What is the average order value (AOV) on Olist, and how does this vary by product category and payment method?
5) How many sellers are active on Olist, and how does this number change over time?
6) What is the distribution of seller ratings on Olist, and how does this impact sales performance?
7) What are the top-selling products on Olist?
8) Which payment methods are most commonly used by Olist customers, and how does this vary by product category or geographic region?
9) Which product categories have the highest profit margins on Olist?
10) What Geolocation has high customer density?
11) Delivery Analysis

**Key Insights**
 1) Olist generated a total revenue of $15.42 million from October 2016 to August 2018. The highest revenue was recorded in November, coinciding with the "Black Friday" 
 festival. Overall, Olist's revenue trend showed a year-by-year increase in addition, Olist processed a total of 96,000 orders. The highest number of orders was received in 
 November.
2) The Average order value (AOV) for the Olist platform is 154.10. This high AOV suggests that customers are buying more expensive products and Tthe credit card is the most preferred payment method for customers.
3) Olist boasts a total of 3,095 sellers, and the trend of active sellers has increased annually. This suggests that Olist provides the best platform for sellers to market their products.
4) Olist has an average review score of 4.09. Analysis indicates that the review score has an impact on both total revenue and orders.
5) Olist offers a total of 74 different products, with the categories of Health & Beauty, Watches & Gifts, and Bed, Bath & Table generating the highest revenue among them all.
6) Credit Cards are the major type of payment used by Olist Customers, followed by Boletos while the least used method is Debit card. This may be due to credit cards being more widely accepted than debit cards. This preferrence may also be due to the convenience and security offered by credit card payments.
7) The gross profit margin for Olist is 14.27%. The product category "Furniture & Decor" generated the highest gross profit margin, and it is also included in the top 10 ordered categories.
8) Customers in the states of São Paulo (SP), Rio de Janeiro (RJ), and Minas Gerais (MG) are characterized by high population density.
9) Olist had a total of 96.48K orders, out of which 7K orders were delivered late to the customers.

**Recommendations:**
1) Olist should implement a seasonal/quarterly promotional events like the "Black Friday" sales to drive customer engagement, high product purchase and increased revenue.
2) Olist should prioritise improving the quality and ensuring timely delivery of its highest revenue-generating products to enhance sales revenue.
3) Focusing on products with lower review scores and working to improve service according to customer feedback can be a strategic approach for earning higher profits and fostering business growth.
4) To leverage the high customer density in São Paulo (SP), Rio de Janeiro (RJ), and Minas Gerais (MG), Olist could implement on-time and free delivery services tailored specifically for these states. Additionally, focusing on marketing and advertising efforts targeted at attracting more customers from these regions can significantly contribute to business growth.
5) The increase in late deliveries in 2018 may be attributed to Olist receiving its highest number of orders during that period. This underscores the need for Olist to focus on delivery services and staff during peak periods to ensure customer satisfaction.

Thank you for your time i'm happy to listen any suggestions.😊👩‍💻

Q1

<img width="579" alt="image" src="https://github.com/Info-Insight/Olist_Store_Analysis/assets/153328845/61f23aaa-07ec-4d47-ad61-d5c33b58d43d">

Q2

<img width="577" alt="image" src="https://github.com/Info-Insight/Olist_Store_Analysis/assets/153328845/357f725a-e69a-47f4-a0d6-caceb37a76b0">

Q3

<img width="578" alt="image" src="https://github.com/Info-Insight/Olist_Store_Analysis/assets/153328845/3e49c579-0692-4133-87dd-a97fa287b72b">

Q4

<img width="572" alt="image" src="https://github.com/Info-Insight/Olist_Store_Analysis/assets/153328845/ed9984a8-ecfe-4943-af48-291bbaccd260">

Q5

<img width="575" alt="image" src="https://github.com/Info-Insight/Olist_Store_Analysis/assets/153328845/f7f140de-fc42-4451-ac00-9801617a6346">


Q6

<img width="579" alt="image" src="https://github.com/Info-Insight/Olist_Store_Analysis/assets/153328845/5147fbb4-6074-40bc-a33d-370f660166b2">

Q7

<img width="575" alt="image" src="https://github.com/Info-Insight/Olist_Store_Analysis/assets/153328845/be74ed22-565e-49f4-8bab-d6ada48cd4a5">

Q8

<img width="580" alt="image" src="https://github.com/Info-Insight/Olist_Store_Analysis/assets/153328845/1381e45b-95e0-44f4-b8ad-360f2ee37178">

Q9

<img width="579" alt="image" src="https://github.com/Info-Insight/Olist_Store_Analysis/assets/153328845/67203701-dd00-4c59-9ff0-94c1fd3c2260">

Q10

<img width="577" alt="image" src="https://github.com/Info-Insight/Olist_Store_Analysis/assets/153328845/474e6abd-5f62-4150-b048-d344e82fa639">

Q11

<img width="576" alt="image" src="https://github.com/Info-Insight/Olist_Store_Analysis/assets/153328845/049d0af4-a32f-41fd-9652-a3b7218b849a">












   





