# Northwind Traders Data Modernization Project

## Overview

Northwind Traders, a global specialty foods export-import company, is undertaking a significant data modernization project. This project aims to transition from a mix of on-premise and legacy systems to a scalable, secure, and efficient cloud-based platform using Google Cloud Platform (GCP), dbt (data build tool), and BigQuery.

## Objectives

- **Modernize Data Architecture:** Migrate from the existing MySQL database to a cloud-based solution on GCP.
- **Enhance Performance:** Resolve current performance bottlenecks caused by using the same MySQL database for transactions and reporting.
- **Improve Scalability and Security:** Implement a scalable architecture and enhance data security and access control.
- **Optimize Reporting:** Reduce load on operational systems and speed up report generation.

## Proposed Solution

- **Cloud Migration:** Transition the existing MySQL database to Google Managed Services Cloud SQL for improved reporting solutions.
- **Data Warehouse Construction:** Develop a dimensional data warehouse on GCP using BigQuery, adopting Kimball's methodology, with dimension and fact tables.
- **OLTP Solution:** Utilize BigQuery as the primary OLTP system to support all reporting requirements.

## Tools and Technologies

- **Google Cloud Platform (GCP):** For hosting the cloud-based data platform.
- **BigQuery:** As the main data warehouse service.
- **dbt (Data Build Tool):** For data transformation, testing, and documentation.

## Implementation Guide

### Prerequisites

1. **Google Cloud Account:** Ensure you have access to Google Cloud Platform.
2. **dbt Installation:** Install dbt core on your machine. Refer to the [dbt installation guide](https://docs.getdbt.com/dbt-cli/installation) for detailed instructions.

### Repository Setup

1. **Clone the Repository:** Clone this repository to your local machine.
2. **Configure dbt:** Set up dbt core with BigQuery. Follow the [dbt setup guide](https://docs.getdbt.com/tutorial/setting-up) for BigQuery.

### Running the Project

Execute the following commands in your terminal after navigating to the project directory:

1. **Run dbt Models:**
```cmd
dbt run
```
This command compiles and runs the data models defined in the project.

2. **Test Data Integrity:**
```cmd
dbt test
```
This ensures the integrity and consistency of the data models.

3. **Generate Documentation:**
```cmd
dbt docs generate
```
This generates documentation for your dbt project, making it easier to understand and navigate the data models.

#
