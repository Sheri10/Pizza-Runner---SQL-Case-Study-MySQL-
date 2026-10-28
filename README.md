# Pizza-Runner---SQL-Case-Study-MySQL-

SQL analysis of a pizza delivery business: cleaning messy order data, measuring pizza and delivery performance, and working out which ingredients are used. This is Case Study #2 of Danny Ma's 8 Week SQL Challenge, solved in MySQL 8.0.

Dataset

Six tables in the pizza_runner database: runners, customer_orders, runner_orders, pizza_names, pizza_recipes and pizza_toppings. The data is intentionally messy (empty strings, the text 'null', distances like 20km, durations like 32 minutes).

What I did
Data cleaning: replaced empty and 'null' values with NULL, removed units from distance and duration, and converted the columns to numeric and date types.
Pizza metrics: pizzas ordered and delivered, orders per customer and orders by day and hour.
Runner and customer experience: signups per week, average pickup time, delivery distance and speed, and the correlation between pizzas per order and preparation time.
Ingredient optimisation: order items such as Meatlovers - Exclude Cheese - Extra Bacon, ingredient lists with 2x, and the quantity of each ingredient used in delivered pizzas.
Bonus: how a new "Supreme" pizza would impact the data design.
Skills

Joins, CTEs, window functions (ROW_NUMBER), aggregate functions, CASE, UNION ALL, string functions for comma-separated lists (FIND_IN_SET, GROUP_CONCAT), date functions (TIMESTAMPDIFF) and data cleaning.

Files
File	Purpose
00_init_pizza_runner_mysql.sql	Creates the database and tables and loads the raw data
pizza_runner_queries.sql	The cleaning steps and the queries
How to run
Run 00_init_pizza_runner_mysql.sql in MySQL Workbench (MySQL 8.0+). It drops and recreates the pizza_runner database.
Run the cleaning steps once, then the queries. To start again, re-run the init script.
Credits

Case study and dataset by Danny Ma. Queries written by me as part of a personal SQL learning project.
