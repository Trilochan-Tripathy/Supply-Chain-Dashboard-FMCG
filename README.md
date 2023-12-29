# Supply-Chain-Dashboard-FMCG
AtliQ Mart is a growing FMCG manufacturer headquartered in Gujarat, India. It is currently operational in three cities Surat, Ahmedabad and Vadodara. They want to expand to other metros/Tier 1 cities in the next 2 years.

AtliQ Mart is currently facing a problem where a few key customers did not extend their annual contracts due to service issues. It is speculated that some of the essential products were either not delivered on time or not delivered in full over a continued period, which could have resulted in bad customer service. Management wants to fix this issue before expanding to other cities and requested their supply chain analytics team to track the ’On time’ and ‘In Full’ delivery service level for all the customers daily basis so that they can respond swiftly to these issues.

The Supply Chain team decided to use a standard approach to measure the service level in which they will measure ‘On-time delivery (OT) %’, ‘In-full delivery (IF) %’, and OnTime in full (OTIF) %’ of the customer orders daily basis against the target service level set for each customer. 

# Task:  
1. Create the metrics according to the metrics list.
2. Create a dashboard according to the requirements provided by stakeholders in the business review meeting. You will be provided with the transcript of this business review meeting in comic form.
3. Create relevant insights not provided in the metric list/stakeholder meeting.

# Dataset :-
This file contains all the meta information regarding the columns described in the CSV files.
1. dim_customers.csv - This table contains all the information about customers
  - customer_id: Unique ID is given to each customer
  - customer_name: Name of the customer
  - city: It is the city where the customer is present

2. dim_products.csv - This table contains all the information about the products
  - product_name: It is the name of the product
  - product_id: Unique ID is given to each of the products
  - category: It is the class to which the product belongs

3. dim_date - This table contains the dates at daily, monthly level and week numbers of the year
  - date: date at the daily level
  - mmm_yy: date at the monthly level
  - week_no: week number of the year as per the date column

4. dim_targets_orders - This table contains all target data at the customer level
  - customer_id: Unique ID that is given to each of the customers
  - ontime_target %: Target assigned for Ontime % for a given customer
  - infull_target %: Target assigned for infull % for a given customer
  - otif_target %:   Target assigned for otif % for a given customer


5. fact_order_lines.csv - This table contains all information about orders and each item inside the orders.
 - order_id: Unique ID for each order the customer placed
 - order_placement_date: It is the date when the customer placed the order
 - customer_id: Unique ID that is given to each of the customers
 - product_id: Unique ID that is given to each of the products
 - order_qty: It is the number of products requested by the customer to be delivered
 - agreed_delivery_date: It is the date agreed between the customer and Atliq Mart to deliver the products
 - actual_delivery_date: It is the actual date Atliq Mart delivered the product to the customer
 - delivered_qty: It is the number of products that are actually delivered to the customer

6. fact_orders_aggregate.csv - This table contains information about OnTime, InFull and OnTime Infull information aggregated at the order level per customer
 - order_id: Unique ID for each order the customer placed
 - customer_id: Unique ID that is given to each of the customers
 - order_placement_date: It is the date when the customer placed the order
 - on_time: '1' denotes the order is delviered on time. '0' denotes the order is not delivered on time.
 - in_full: '1' denotes the order is delviered in full quantity. '0' denotes the order is not delivered in full quantity.
 - otif:    '1' denotes the order is delviered both on time and in full quantity. '0' denotes the order is either not delivered on time or not in full quantity.




# Live Dashboard :- 
https://app.powerbi.com/groups/me/reports/1537bba0-c8a5-4ba5-9ae1-ddae2a239024/ReportSection15034c303830d314a329?experience=power-bi 

# NovyPro :-
https://app.powerbi.com/groups/me/reports/1537bba0-c8a5-4ba5-9ae1-ddae2a239024/ReportSection15034c303830d314a329?experience=power-bi 

# Home Page:-
<img width="604" alt="image" src="https://github.com/Trilochan-Tripathy/Supply-Chain-Dashboard-FMCG/assets/141568396/64e27f7e-afb9-4262-adb1-04a792f691d3">

# City Performance :-
<img width="552" alt="image" src="https://github.com/Trilochan-Tripathy/Supply-Chain-Dashboard-FMCG/assets/141568396/89f50bb1-75c1-4811-8d3a-034d93fca8de">

# Product View :-
<img width="604" alt="image" src="https://github.com/Trilochan-Tripathy/Supply-Chain-Dashboard-FMCG/assets/141568396/66e5ed00-8403-4f48-acf9-d44a0459c32b">

# Customer Performance :-
<img width="606" alt="image" src="https://github.com/Trilochan-Tripathy/Supply-Chain-Dashboard-FMCG/assets/141568396/af4304df-063c-4495-9fcf-8e61ad96a797">



