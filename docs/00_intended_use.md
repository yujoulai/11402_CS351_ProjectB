# 00 Intended Use

## 1. Project Purpose

Project B aims to design and implement a lightweight CSV Mini Database & Query Engine that can read CSV files, parse structured data, and support simplified command-line queries.

The project focuses on core educational database functions such as data loading, filtering, and column selection rather than full-scale database system development.

---

## 2. Target Users

This project is intended for:

* Students learning software engineering and system design
* Instructors evaluating CLI-based project workflows
* Developers practicing structured data parsing

Users are expected to have basic command-line knowledge.

---

## 3. Execution Environment

The system is expected to run in:

* C++
* Command-line interface (CLI)
* Windows, Linux, or macOS
* CMake-based build environment

The project should build and run from a clean setup with minimal dependencies.

---

## 4. Input and Output Expectations

### Input:

* CSV files with header-defined columns
* Structured comma-separated records
* User-entered CLI queries

### Output:

* Parsed data
* Filtered query results
* Selected columns
* Clear error messages for invalid input or unsupported operations

---

## 5. Success Criteria

The project is successful if it can:

* Load and parse valid CSV files
* Preserve data structure correctly
* Execute basic query commands
* Return accurate results
* Handle invalid input predictably
* Build and run successfully from documented instructions

---

## 6. Explicit Non-Goals

This project does NOT aim to:

* Support full SQL syntax
* Implement joins or advanced relational features
* Provide GUI support
* Serve as a production-grade DBMS
* Optimize for large-scale systems

---

## 7. Constraints

The project must:

* Follow course SOP and Git workflow
* Maintain clear documentation and traceability
* Prioritize modular design
* Minimize unnecessary dependencies
* Remain within course scope and timeline
