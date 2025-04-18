Sales Data Analysis with SQLite and Python
*Project Description
This project showcases how to perform basic sales data analysis using a combination of SQLite, Python, pandas, and matplotlib. It simulates a simple retail scenario where sales transactions are stored in a local database, and insights like total quantity sold and revenue generated per product are derived through SQL queries and visualized using bar charts.
* Step-by-Step Workflow
  --Import Required Libraries
    The code begins by importing essential libraries:
    sqlite3 for database operations
    pandas for data handling and analysis
    matplotlib.pyplot for visualization
 --Create/Connect to SQLite Database
   A connection is established to a local SQLite database file named sales_data.db. If the file doesn’t exist, it will be created automatically.
 --Create Sales Table
   A table named sales is created (if it doesn’t already exist) with the following columns:
   id: Unique identifier (Primary Key)
   product: Name of the product
   quantity: Quantity sold
   price: Price per unit
--Insert Sample Data
  Sample records of products like Apple, Banana, and Orange are inserted into the table. This step simulates real-world sales transactions.
--SQL Query for Aggregated Analysis
  A SQL query is used to group the data by product and calculate:
  total_qty: Total quantity sold per product
  revenue: Total revenue (quantity × price), rounded to 2 decimal places
  The result is stored in a pandas DataFrame for further processing.
--Display the Summary
  The aggregated sales summary is printed to the console for a quick overview.
--Visualize Revenue Data
  A bar chart is plotted to visualize revenue per product using matplotlib. The chart:
  Highlights revenue for each product
  Includes labels and grid for better readability
  Additionally, the chart is saved as an image file named sales_chart.png.
--Close the Database Connection
  Finally, the connection to the database is closed to free up system resources.


