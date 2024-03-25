
Analyzing International Debt Statistics Using SQL
This project focuses on analyzing international debt statistics using SQL queries. The dataset used contains information about the amount of debt (in USD) owed by developing countries across different categories such as external debt, public sector debt, and private sector debt.

Dataset Description
The dataset used in this project contains the following columns:

country_name: Name of the country.
country_code: ISO code of the country.
indicator_name: Name of the debt indicator.
indicator_code: Code of the debt indicator.
year: Year for which the debt data is recorded.
debt: Amount of debt in USD.
Analysis Objectives
The main objectives of this analysis include:

Identifying the countries with the highest debt.
Analyzing the trend of debt accumulation over the years.
Comparing debt statistics across different regions and income groups.
Investigating the distribution of debt across various debt indicators.
SQL Queries
To achieve the analysis objectives, the following SQL queries will be executed:

Identifying Top Debtors:

Query to retrieve the top countries with the highest debt amounts.
Analyzing Debt Trend:

Query to calculate the total debt amount for each year to analyze the trend of debt accumulation over time.
Comparing Debt by Region and Income Group:

Queries to compare debt statistics across different regions and income groups.
Investigating Debt Distribution by Indicator:

Query to analyze the distribution of debt across different debt indicators.
Instructions
Setup SQL Environment:

Ensure that you have access to a SQL database management system (DBMS) such as MySQL, PostgreSQL, or SQLite.
Load Dataset:

Import the provided dataset (debt_data.csv) into your SQL database management system.
Execute SQL Queries:

Run the SQL queries provided in the queries.sql file against the loaded dataset to perform the desired analysis.
Interpret Results:

Analyze the results obtained from the SQL queries to gain insights into international debt statistics.
Example Queries
Below are examples of SQL queries that can be used for analysis:

sql
Copy code
-- Query to retrieve top debtors
SELECT country_name, SUM(debt) AS total_debt
FROM debt_data
GROUP BY country_name
ORDER BY total_debt DESC
LIMIT 10;
sql
Copy code
-- Query to calculate total debt by year
SELECT year, SUM(debt) AS total_debt
FROM debt_data
GROUP BY year
ORDER BY year;
Conclusion
Analyzing international debt statistics using SQL provides valuable insights into the financial health of countries and regions. By executing SQL queries on the dataset, trends, patterns, and correlations can be identified to inform policy decisions and strategic planning.

License
This project is licensed under the MIT License.

Author
[Your Name]

Acknowledgments
International Monetary Fund (IMF) for providing the debt dataset.
SQL community for valuable resources and support.
