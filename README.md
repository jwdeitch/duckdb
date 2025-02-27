<div align="center">
  <img src="https://duckdb.org/images/DuckDB_Logo_dl.png" height="50">
</div>
<p>&nbsp;</p>

<p align="center">
  <a href="https://github.com/duckdb/duckdb/actions">
    <img src="https://github.com/cwida/duckdb/workflows/.github/workflows/main.yml/badge.svg?branch=master" alt=".github/workflows/main.yml">
  </a>
  <a href="https://www.codefactor.io/repository/github/cwida/duckdb">
    <img src="https://www.codefactor.io/repository/github/cwida/duckdb/badge" alt="CodeFactor"/>
  </a>
  <a href="https://app.codecov.io/gh/duckdb/duckdb">
    <img src="https://codecov.io/gh/duckdb/duckdb/branch/master/graph/badge.svg?token=FaxjcfFghN" alt="codecov"/>
  </a>
  <a href="https://discord.gg/tcvwpjfnZx">
    <img src="https://shields.io/discord/909674491309850675" alt="discord" />
  </a>
</p>f

## DuckDB
DuckDB is a high-performance analytical database system. It is designed to be fast, reliable and easy to use. DuckDB provides a rich SQL dialect, with support far beyond basic SQL. DuckDB supports arbitrary and nested correlated subqueries, window functions, collations, complex types (arrays, structs), and more. For more information on the goals of DuckDB, please refer to [the Why DuckDB page on our website](https://duckdb.org/docs/why_duckdb.html).

## Installation
If you want to install and use DuckDB, please see [our website](https://www.duckdb.org) for installation and usage instructions.

## Data Import
For CSV files and Parquet files, data import is as simple as referencing the file in the FROM clause:

```sql
SELECT * FROM 'myfile.csv';
SELECT * FROM 'myfile.parquet';
```

Refer to our [Data Import](https://duckdb.org/docs/data/overview) section for more information.

## SQL Reference
The [website](https://duckdb.org/docs/sql/introduction) contains a reference of functions and SQL constructs available in DuckDB.

## Development 
For development, DuckDB requires [CMake](https://cmake.org), Python3 and a `C++11` compliant compiler. Run `make` in the root directory to compile the sources. For development, use `make debug` to build a non-optimized debug version. You should run `make unit` and `make allunit` to verify that your version works properly after making changes. To test performance, you can run several standard benchmarks from the root directory by executing `./build/release/benchmark/benchmark_runner`.

Please also refer to our [Contribution Guide](CONTRIBUTING.md).


