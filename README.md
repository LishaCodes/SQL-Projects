## This project focuses on analyzing e-commerce data to uncover customer purchasing patterns. We utilize Python for data manipulation and PostgreSQL for database management. Below is a detailed description of the methodology and process followed in this project.

## Methodology

1. Data Loading:
We load data from CSV files into pandas DataFrames. The datasets include orders, aisles, departments, order products, and products.

2. Data Sampling:
To optimize performance and handleability, we sample 10,000 rows from the orders and order_products datasets.

3. Database Connection:
We establish a connection to a PostgreSQL database using psycopg2 and SQLAlchemy.

5. Database Schema Creation:
We create tables in the PostgreSQL database to store the datasets. The tables include:
i. aisles
ii. departments
iii. products
iv. orders
v. order_products

6. Data Cleaning:
We drop the 'eval_set' column from the orders dataset as it is not needed for our analysis.

7. Data Insertion:
We use the SQLAlchemy to_sql method to insert data from the pandas DataFrames into the PostgreSQL tables.
