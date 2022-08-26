## SEC API portion

Notes to self:

* Find the source code which scrapes the *Summary Compensation Table* and see if it can be extended to the other pay tables
    * Grants of Plan-Based Awards
    * Options Exercised and Stock Vested
    * Outstanding Awards

* Navigate the 10-K (and 10-Q, etc.) dictionaries to pull the relevant financial information into DataFrames
  * For example, figure out the appropriate dictionary keys for isolating and labeling the values for "Revenue" and "Outstanding Shares" and "Current Assets" and so on

* Rather than converting each query to a separate CSV file, store them in a database. Modify the original query function to directly add new JSON query results (or a subsequent DataFrame) to a database.
  * https://www.geeksforgeeks.org/how-to-convert-pandas-dataframe-into-sql-in-python/
  * https://blog.jcharistech.com/2020/01/08/how-to-convert-json-to-sql-format-in-python/
  * https://stackoverflow.com/questions/40450591/converting-json-to-sql-table
  * https://stackoverflow.com/questions/48604563/creating-a-data-structure-from-json-using-python
