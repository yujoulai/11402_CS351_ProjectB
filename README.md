# Project B - CSV Mini Database & Query Engine

## 1. Project Overview

This project aims to implement a lightweight CSV-based mini database system with a simple query engine.
Instead of building a full DBMS, the goal is to simulate core database functionalities such as data loading, parsing, filtering, and querying using CSV files.

The system will read structured data from CSV files and allow users to perform basic queries to retrieve specific information.

---

## 2. Objectives

The objectives of this project are:

* To design and implement a CSV parser
* To build a simple query engine for data retrieval
* To support basic filtering and column selection
* To understand data organization and query processing
* To practice modular software design and Git-based development workflow

---

## 3. Planned Features

The system is expected to support the following features:

* Load and read CSV files
* Parse headers and data records
* Store data in an appropriate in-memory structure
* Select specific columns from the dataset
* Filter rows based on conditions
* Display query results in a readable format
* Handle invalid inputs and edge cases

---

## 4. System Design

The overall system is designed as a pipeline:

CSV File → CSV Parser → Data Storage → Query Engine → Output

* **CSV Parser**: Responsible for reading and parsing CSV files
* **Data Storage**: Stores parsed data in memory
* **Query Engine**: Processes user queries and retrieves matching records
* **Output Module**: Formats and displays results

This modular design improves maintainability and scalability.

---

## 5. File Structure (Planned)

The project is expected to follow the structure below:

```
/src
  main.cpp
  csv_parser.cpp
  query_engine.cpp

/include
  csv_parser.h
  query_engine.h

/data
  sample.csv
```

* `main.cpp`: Entry point of the program
* `csv_parser`: Handles CSV file reading and parsing
* `query_engine`: Handles query processing and execution

---

## 6. Data Structure (Design)

The data will be stored in memory using standard data structures:

* Header: `vector<string>`
* Rows: `vector<vector<string>>`

Each row represents a record, and each column corresponds to a field defined in the header.

Future improvements may include more structured representations (e.g., structs or classes).

---

## 7. Expected Usage

The system is expected to be executed from the command line:

```
./mini_db data/sample.csv
```

Users will then input queries to retrieve data from the CSV file.

---

## 8. Query Syntax (Draft)

The query system will follow a simplified SQL-like format.

### Basic format:

```
SELECT column_name WHERE condition
```

### Examples:

```
SELECT name
SELECT name, age WHERE age > 20
SELECT id WHERE id = 1001
```

### Supported operations (planned):

* Comparison: `=`, `>`, `<`
* Column selection
* Single-condition filtering

More advanced query features may be added in future versions.

---

## 9. Development Plan

The project will be developed in the following phases:

* **Phase 1**: CSV file reading and parsing
* **Phase 2**: Data storage implementation
* **Phase 3**: Query parsing
* **Phase 4**: Query execution
* **Phase 5**: Testing and validation

Each phase will be implemented incrementally with version control using Git.

---

## 10. Future Work

Possible future improvements include:

* Support for multiple conditions (AND / OR)
* Sorting results
* Aggregation functions (COUNT, AVG, etc.)
* More robust CSV parsing (handling quotes, commas in fields)
* Interactive command-line interface improvements

---

## 11. Development Workflow

This project follows a Git-based workflow:

* Development will be done in feature branches
* Changes will be committed with descriptive messages
* Pull requests will be used for integration
* Code will be reviewed before merging

This ensures structured and traceable development progress.

---

## 12. Status

This project is currently in the **initialization and design phase**.
Core functionalities are under development.
