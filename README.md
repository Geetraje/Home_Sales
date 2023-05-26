# Home_Sales
This challenge uses SparkSQL to determine key metrics about home sales data in addition to using Spark to create temporary views, partition data, cache and uncahe a temporary table and verify that the table has been cached.

It is a small demonstration of the advantages of using Apache Spark and its module SparkSQL in analyzing large scale data in a short time.

# Process
## Using SparkSQL to wrangle data

- What is the average price for a four-bedroom house sold for each year? Round off your answer to two decimal places.

![image](https://github.com/Geetraje/Home_Sales/assets/119769357/eb1cf4c3-960a-47a1-96a2-995086ea029e)

- What is the average price of a home for each year it was built that has three bedrooms and three bathrooms? Round off your answer to two decimal places.

![image](https://github.com/Geetraje/Home_Sales/assets/119769357/58594354-21aa-4b59-9b0c-710cfa792b70)

- What is the average price of a home for each year that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet? Round off your answer to two decimal places.

![image](https://github.com/Geetraje/Home_Sales/assets/119769357/503c7afa-b3b6-46f3-af88-d4f22ad3e57d)

- What is the "view" rating for homes costing more than or equal to $350,000? Determine the run time for this query, and round off your answer to two decimal places.

``Uncached Data``

![image](https://github.com/Geetraje/Home_Sales/assets/119769357/945d6178-6c6e-41db-b688-4e8fde8c1435)


- What is the "view" rating for homes costing more than or equal to $350,000? Determine the run time for this query, and round off your answer to two decimal places.

``Cached Data``

![image](https://github.com/Geetraje/Home_Sales/assets/119769357/28225ab7-688c-42b5-a51c-6f822f0985e5)


# Results
- The query on the uncached view used a run time of 7.29 secs whereas Cache-ing the table and running the same query provided the results in 4.69 secs. 
- Partitioning the parquet format reduced the run time on the same query to 4.29secs

# Conclusion
- Caching and Partitioning data with Spark increases efficiency of SQL queries by speeding up the process. 
- This would be very useful when dealing with big datasets.
