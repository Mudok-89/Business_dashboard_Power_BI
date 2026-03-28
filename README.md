# Business Dashboard | Power BI

Interactive business dashboard created in Power BI for management reporting based on the Classic Models dataset stored in a MySQL database.

## Project background
The goal of this project was to build a comprehensive business dashboard for company management. The dashboard provides an overview of key business results and allows users to compare performance across regions, employees, offices, and time periods.

The project is based on the **Classic Models** dataset from a MySQL database and includes data about offices, employees, customers, orders, payments, products, product lines, and order details.

## Business goal
The dashboard is designed to help managers:
- monitor key business KPIs
- compare results across time periods
- analyze sales and payments by region
- evaluate employee and office performance
- identify trends and seasonal patterns

## Data sources

The project is based on source data exported from the MySQL schema `exam14_99`. The original source file names were preserved to reflect the structure of the database tables.

Main source files:
- `exam14_99_customers.csv`
- `exam14_99_employees.csv`
- `exam14_99_offices.csv`
- `exam14_99_orderdetails.csv`
- `exam14_99_orders.csv`
- `exam14_99_payments.csv`
- `exam14_99_productlines.csv`
- `exam14_99_products.csv`

The original source file names were preserved to reflect the structure of the source database tables.

## Data preparation
Data was imported from MySQL into Power BI and transformed in Power Query.

Main preparation steps included:
- cleaning and formatting data types
- merging and shaping selected fields
- building relationships between tables
- creating a custom time column for month / year-month from `orderDate` or `paymentDate`
- preparing data for time-based comparison and filtering

## Dashboard content

### Main KPIs
The dashboard includes key business indicators such as:
- total received payments
- total number of orders
- average payment amount or average order value
- total number of customers
- total sales

### Visualizations
The dashboard contains multiple visualization types, for example:
- line chart for orders and payments over time
- bar charts for office and employee performance
- map or regional view for geographic comparison
- pie or category charts for product lines or sales structure

## Time comparison
A custom month / year-month column was created to support period-over-period analysis.

This makes it possible to:
- compare results between months
- track development over time
- identify trends and seasonal effects
- filter dashboard results by selected periods

## DAX measures
The project includes custom measures for business reporting, such as:
- total payments
- order count
- average order value
- average payment amount
- customer count
- dynamic metrics changing based on filters and slicers

Additional calculations can include:
- growth between selected periods
- comparisons across regions
- filtered KPIs based on user interaction

## Interactivity
The dashboard uses slicers and filters for:
- time period
- region / country / city / office
- employee
- product line

This allows managers to explore results interactively and compare business performance from different perspectives.

## Business value
This dashboard helps management:
- get a fast overview of company performance
- compare offices, regions, and employees
- detect stronger and weaker business areas
- monitor time-based performance changes
- support data-driven decision-making

## Files in this repository
- `README.md` – project overview and documentation
- `DashBoard Class Models.pbix` – Power BI dashboard file
- `project_brief_CZ.pdf` – project brief in Czech
- `project_brief_en.pdf` – project brief in English
- `data/` – source CSV files used in the dashboard
- `data/README.md` – additional notes related to source data files

## Skills demonstrated
- Power BI
- Power Query
- DAX
- data modeling
- KPI design
- dashboard design
- time-series analysis
- interactive filtering
- MySQL data connection
- business reporting
- management-oriented data visualization

## Notes
This project was created as a business intelligence and reporting exercise focused on transforming raw relational data into an interactive dashboard for management use.

