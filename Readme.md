###Home Sales Big Data with PySpark and SQL

Through utilizing PySpark and Spark SQL on Google Colab, this project serves to determine key metrics about home sales data. Then, Spark is utilized to create temporary views, partition the data, cache and uncache a temporary table. Some of the data key metric questions that were answered:

**Question 1: What is the average price for a four-bedroom house sold for each year? Round off your answer to two decimal places.**

**Answer 1:**
+--------------------+----------+
|round(avg(price), 2)|year(date)|
+--------------------+----------+
|           296363.88|      2022|
|           301819.44|      2021|
|           298353.78|      2020|
|            300263.7|      2019|
+--------------------+----------+

**Question 2: What is the average price of a home for each year it was built that has three bedrooms and three bathrooms? Round off your answer to two decimal places.**
**Answer 2:** 
+--------------------+----------+
|round(avg(price), 2)|date_built|
+--------------------+----------+
|           292676.79|      2017|
|           290555.07|      2016|
|            288770.3|      2015|
|           290852.27|      2014|
|           295962.27|      2013|
|           293683.19|      2012|
|           291117.47|      2011|
|           292859.62|      2010|
+--------------------+----------+

**Question 3: What is the average price of a home for each year that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet? Round off your answer to two decimal places.**
**Answer 3:** 
+--------------------+----------+
|round(avg(price), 2)|date_built|
+--------------------+----------+
|           280317.58|      2017|
|            293965.1|      2016|
|           297609.97|      2015|
|           298264.72|      2014|
|           303676.79|      2013|
|           307539.97|      2012|
|           276553.81|      2011|
|           285010.22|      2010|
+--------------------+----------+

**Question 4: What is the "view" rating for homes costing more than or equal to $350,000? Determine the run time for this query, and round off your answer to two decimal places.**
**Answer 4:** The query runtime for this question is approximately 0.49 seconds, and the "view" ratings for homes costing more than or equal to $350,000 are as follows:
+----+--------------------+
|view|round(avg(price), 2)|
+----+--------------------+
|  51|           788128.21|
|  54|           798684.82|
|  69|           750537.94|
|  87|           1072285.2|
|  73|           752861.18|
|  64|           767036.67|
|  59|            791453.0|
|  85|          1056336.74|
|  52|           733780.26|
|  71|            775651.1|
|  98|          1053739.33|
|  99|          1061201.42|
|  96|          1017815.92|
| 100|           1026669.5|
|  70|           695865.58|
|  61|           746877.59|
|  75|          1114042.94|
|  78|          1080649.37|
|  89|          1107839.15|
|  77|          1076205.56|
+----+--------------------+
only showing top 20 rows



