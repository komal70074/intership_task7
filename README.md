# intership_task7


Dataset:
Create a small SQLite database file (sales_data.db) with just one sales table
Deliverables:
Python script (or notebook) that:
Connects to sales_data.db
Runs 1–2 SQL queries
Displays output using print and basic matplotlib bar chart
Hints / Mini Guide:
Load SQLite database: import sqlite3 conn = sqlite3.connect("sales_data.db")
Run basic SQL: query = "SELECT product, SUM(quantity) AS total_qty, SUM(quantity * price) AS
revenue FROM sales GROUP BY product"
Load into pandas: import pandas as pd df = pd.read_sql_query(query, conn)
Print results: print(df)
Plot simple bar chart: df.plot(kind='bar', x='product', y='revenue')
Save chart if needed: plt.savefig("sales_chart.png")
