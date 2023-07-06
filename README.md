**Tested Business Intelligence(BI) Engines(ChDB & DuckDB)**

*Description*   
- Tested & compared performance for SQL OLAP(Online Analytical Processing) engines namely chDB and DuckDB, using the TPCH_SF10 decision support queries
-	Executed a series of 22 complex SQL queries against large datasets to assess the engines' query execution times, resource utilization and overall performance
-	Wrote python script to compare the performance of both engines & visualized results using Matplotlib

*Findings*
- Currently, chDB(the embedded version of the clickhouse dbms) only supports Python 3.8+ on macOS(x86_64 and ARM64) and Linux
- Both chDB and duckDB don't need full server installation. Its easier to get started just by importing the required module from python library
- DuckDB can ingest data from a wide variety of formats. Running SQL queries is very straight forward just using the duckdb.sql command
- Querying over millions of rows, I found duckDB was faster than chDB

TPC-H reference: http://tpc.org/tpc_documents_current_versions/pdf/tpc-h_v3.0.0.pdf
