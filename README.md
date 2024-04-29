# Home_Sales
Module 22 Challenge - UWA Data Analytics Bootcamp

This repository contains main code found in the file "Home_Sales_Main_Code_Colab.ipynb", which performs analysis on home sales data.

The average price for a four bedroom house for each sell year was:
+---------+-------------+
|YEAR_SOLD|AVERAGE_PRICE|
+---------+-------------+
|     2022|    296363.88|
|     2021|    301819.44|
|     2020|    298353.78|
|     2019|     300263.7|
+---------+-------------+

The average price of a 3 bedroom and 3 bathroom house for each build year was:
+----------+-------------+
|BUILD_YEAR|AVERAGE_PRICE|
+----------+-------------+
|      2017|    292676.79|
|      2016|    290555.07|
|      2015|     288770.3|
|      2014|    290852.27|
|      2013|    295962.27|
|      2012|    293683.19|
|      2011|    291117.47|
|      2010|    292859.62|
+----------+-------------+

The average price for a home with 3 bedrooms and 3 bathrooms, 2 floors and >= 2000 square feet per build year was:
+----------+-------------+
|BUILD_YEAR|AVERAGE_PRICE|
+----------+-------------+
|      2017|    280317.58|
|      2016|     293965.1|
|      2015|    297609.97|
|      2014|    298264.72|
|      2013|    303676.79|
|      2012|    307539.97|
|      2011|    276553.81|
|      2010|    285010.22|
+----------+-------------+

The average price per view rating for homes with a price greater or equal to $350,000 was (top 20 VIEW_RATINGs only):
+-----------+-------------+
|VIEW_RATING|AVERAGE_PRICE|
+-----------+-------------+
|         99|   1061201.42|
|         98|   1053739.33|
|         97|   1129040.15|
|         96|   1017815.92|
|         95|    1054325.6|
|         94|    1033536.2|
|         93|   1026006.06|
|         92|    970402.55|
|         91|   1137372.73|
|         90|   1062654.16|
|         89|   1107839.15|
|         88|   1031719.35|
|         87|    1072285.2|
|         86|   1070444.25|
|         85|   1056336.74|
|         84|   1117233.13|
|         83|   1033965.93|
|         82|    1063498.0|
|         81|   1053472.79|
|         80|    991767.38|
+-----------+-------------+

This query had a runtime of 1.48 seconds.
Running the same query after caching the table yielded a runtime of 0.53 seconds.
Running the same query after saving then reading the table in parquet format yielded a runtime of 0.73 seconds.

The best performing method was caching, with the parquet data also being a significant improvement on the original runtime. On larger sets of data, this would make a sizeable time and computation resource difference.