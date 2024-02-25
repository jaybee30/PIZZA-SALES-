**PIZZA-SALES**

**OVERVIEW OF THE DATASET**

Things are going OK here at Plato's, but there's room for improvement. They've been collecting transactional data for the past year, but really haven't been able to put it to good use. Hoping we can analyze the data and put together a report to help us find opportunities to drive more sales and work more efficiently.

**DATA DICTIONARY**

This pizza sales dataset make up 12 relevant features:
order_id: Unique identifier for each order placed by a table
order_details_id: Unique identifier for each pizza placed within each order (pizzas of the same type and size are kept in the same row, and the quantity increases)
pizza_id: Unique key identifier that ties the pizza ordered to its details, like size and price
quantity: Quantity ordered for each pizza of the same type and size
order_date: Date the order was placed (entered into the system prior to cooking & serving)
order_time: Time the order was placed (entered into the system prior to cooking & serving)
unit_price: Price of the pizza in USD
total_price: unit_price * quantity
pizza_size: Size of the pizza (Small, Medium, Large, X Large, or XX Large)
pizza_type: Unique key identifier that ties the pizza ordered to its details, like size and price
pizza_ingredients: ingredients used in the pizza as shown in the menu (they all include Mozzarella Cheese, even if not specified; and they all include Tomato Sauce, unless another sauce is specified)
pizza_name: Name of the pizza as shown in the menu


**Business Tasks**
1.	What days and times do we tend to be busiest?
2.	How many pizzas are we making during peak periods?
3.	What are our best and worst-selling pizzas?
4.	What's our average Revenue?
5.	What is our monthly order performance?
6.	What is the order performance of our various pizza sizes?
7.	Which of our Pizza Category is the most in demand?
8.	What is our monthly revenue performance?
9.	Provide a quick visualization for the Month on Month breakdown of our Revenue vs Orders

   
**Analysis**

Analysis was done on MSSQL and visualized on Power BI. I uploaded the dataset first on SQL Server, queried the dataset to generate insights. 

**INSIGHTS**

The busiest days are Fridays, Thursdays and Sartuday (Beginning of the weekend). Fridays had a total of 3,538 distinct orders, 8,242 quantities of pizzas made, and revenue generation of $136,073.9. While on Thurdays, a total of 3,239 distinct orders were received, a total of 7,478 pizzas made and revenue generation of $123,182.4. For Saturdays, a total of 3,158 distinct orders were made, 7,493 quantities of pizza were made and a total revenue of $123,182.40 was generated.

Overall best selling pizza is The Classic Deluxe Pizza. It was ordered 2,329 times, a total of 2,453 quanties was sold and generated revenue of $38,180.5. The worst selling pizza is The Brie Carre Pizza with a total of just 480 orders, 490 quantities made and revenue of $11,588.5. 
One thing to note is that: the Classic Deluxe pizza is not the best pizza in terms of Revenue, The Thai Chicken Pizza generated a total of $43,434.25 as compared to The Classic Deluxe Pizza which generated revenue of $38,180.5.

July is the top performing month with a total of 1,935 distinct orders, revenue generation of $72,557.9. The least performing month is October with 1,646 distinct orders, 3,883 quantities of pizza sold and revenue generation of $64,027.6.

pizza size is the Large Size with a total of 12,736 (36.43%) orders placed for it, 18,956 quantites sold and revenue generation of $375,318.7. Next is the Medium pizza with a total of 11,159 (31.92%) orders, 15,635 quanties sold, and revenue generation of $249,382.25. Regular/small pizza size with a total of 10,490 (30.01%), 14,403 quantities sold and revenue generation of $178,076.50. X-Large (Extra large) with a total of 544 (1.56%) orders, 552 quantities sold and revenue generation of $14,076.00. The least sold pizza size is the XXL with just 28 (0.08%) orders, 28 quantities sold and $1,006.6 revenue generated.

The pizza category which is most in demand is the Classic with 14,888 quantities sold and $220,053.1 revenue generated while the least pizza category in demand is the Chicken with 11,050 quantities and a revenue of $195,919.50.
It is important to note that Veggie pizza catgory had more quantities of pizza ordered but still contributed a lesser revenue of $193,690.45 as compared to Chicken pizza category.

Our best month in terms of Revenue is July with a total of $72,557.9

**KPIs**
Year considered - 2015
Total Orders - 48,620
Total distinct ordrers - 21,350
Number of pizza types - 32
Number of pizza category - 4
Total Pizza Sold - 49,574
Total revenue - $817,860.05
Average Sales revenue - $16.50
Average order value - 38.31
Average pizzas per order - 2.32

**RECOMMENDATION**
Pizza orders and revenue shows an increasing rate from Sunday and peaks on Friday, then it starts dropping. This indicates that customers have a preference of ordering pizza during the beginning of weekend till saturday evening. It is recommended that all factors of production should be given utmost attention to so as to accomodate the large influx of orders. 

I reecommend that the Extra-large pizza category be scraped since it is a poor performing category having contributed 0.08% of the total orders, a poor revenue of $1,006 and a total of 28 quantity of pizzas in total. The factors of production used on producing this category if used on high performance category will add to the revenue generated.

The Ingredients for Pepperoni pizza should be made readily available and in large quantities on or before Fridays. Since more orders are received on Fridays, a discount policy can be introduced every last Friday of the month where a customer gets 1 extra pizza when they buy 3 and above, this will encourage them to buy more


**DASHBOARD**
![Order](https://github.com/jaybee30/PIZZA-SALES-/assets/106179938/6b74ba6f-afd0-41ed-9e6a-16445f3996ba)
![Best/worst sellers](https://github.com/jaybee30/PIZZA-SALES-/assets/106179938/ba0001ea-79d7-4d95-9794-c5464f0c7f07)
![Revenue](https://github.com/jaybee30/PIZZA-SALES-/assets/106179938/e628704d-278f-4d4b-a818-4c5561b396b7)

THE LINK TO THE INTERACTIVE DASHBOARD CAN BE FOUND BELOW:
https://app.powerbi.com/view?r=eyJrIjoiZGQwYzA5MzAtZTg2YS00OTdhLThjYzgtZGQ1NGQ0MjIyZjIxIiwidCI6IjMyZTBkNjM5LTczMmItNDZhMi05ODFhLTFhZTRkNDJlMDkwNiJ9

