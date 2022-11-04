# What is Amazon Athena?

- Interactive query service to analyze data in Amazon Simple Storage Service (S3) uing standard SQL
- No inrastructure to set up or manage and no data to load (serverless)
- Zero setup cost, just point to Amazon S3 and start querying
- You only pay for the queries you run
- DDL queries and failed queries are free

# Athena Object Model

- You can run DDL statements in the Athena console, using a JDBC or an ODBC driver, or using the Athena Create Table wizard
- When you create a new table schema in Athena, Athens stores the schema in a data catalog and uses it when you run queries
- Athena uses an approach known as **schema-on-read**, which means a schema is projected on to your data at the time you execute a query. This eliminates the need for data loading or transformation
- Athena does not modify your data in Amazon S3
- Athena uses Apache Hive to define tables and create databases, which are essentially a logical namespace of tables
- Athena query engine is based on Hive DDL
- When you query, you query the table using standard SQL and the data is read at that time
- The maximum query string length is 256 KB
- Hive supports multiple data formats through the use of serializer-deserializer(SerDe) libraries.
- You can also define complex schemas using regular expressions
- Athena stores query results in Amazon S3
- Athena lets you create arrays, concatenate them, convert them to different data types, and then filter, flatten, and sort them

# Athena Console Features

- Create or select a database
- Create, view, and delete tables
- Filter tables by starting to type their names
- Preview tables and generate CREATE TABLE DDL for them
- Show table properties
- Run queries on tables, save and format queries, and view query history
- Create up to 10 queries using different query tabs in the query editor
- Display qiery results, save and export them
- Access the AWS Glue Data Catalog
- View abd change settings, such as view the query result location, configure auto-complete, and encrypt query results
