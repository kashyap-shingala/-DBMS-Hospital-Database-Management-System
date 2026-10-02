# Hospital Database Management System (DBMS)

## Overview
This repository contains the database design, relational schema, and SQL project files for a comprehensive Hospital Database Management System. The project is designed to handle core healthcare operations, including patient tracking, staff and doctor assignments, pharmacy inventory, and medical billing.

## Project Documentation
The database architecture has been carefully designed and normalized. You can view the visual design documents in this repository:
* **Entity-Relationship Diagram (ERD):** The conceptual layout of the database entities and their relationships can be found in `T03_DBMS_PROJECT_page-0001.jpg`.
* **Relational Schema:** The detailed schema, including all primary keys, foreign keys, and specific `VARCHAR`, `INT`, `DATE`, and `DECIMAL` data types, is located in `T03_DBMS_PROJECT_page-0002.jpg`
* **Normalization Proofs:** The database design includes rigorous normalization proofs defining the candidate keys and functional dependencies for all tables.

## Database Structure
The database is built on 13 normalized tables to ensure data integrity:

* **Administration & Human Resources**
  * **Department:** Tracks department IDs, names, and locations.
  * **Staff:** Stores employee details including roles, salaries, hire dates, and contact information.
  * **Doctor:** Links to staff profiles while tracking medical specialization, experience, and consultation room assignments.

* **Patient Care & Records**
  * **Patient:** Manages patient demographics, medical history, and insurance information.
  * **Appointment:** Schedules patient visits with specific doctors and tracks the appointment status.
  * **Prescription:** Records prescribed medicines, dosages, and usage frequencies for patients.
  * **LabTestReport:** Tracks laboratory tests, test types, dates, and the resulting reports.
  * **Room:** Manages hospital bed allocations, admission/discharge dates, and daily charges.

* **Pharmacy & Inventory**
  * **Medicine & Medicine_detail:** Manages the pharmacy's medication inventory, including strength, categories, batch numbers, and expiry dates.
  * **Equipment:** Tracks hospital equipment types, warranty periods, and required storage temperatures.
  * **Supplier:** Maintains contact information for the external suppliers of medicines and equipment.

* **Billing**
  * **Invoice:** Handles patient billing, tracking invoice amounts, payment methods, and payment statuses.

## Setup & Installation
*(Note: Add your specific SQL setup instructions here, e.g., how to run your `.sql` scripts to create tables and insert mock data).*

1. Clone this repository to your local machine.
2. Open your preferred SQL environment (e.g., MySQL Workbench, PostgreSQL, SQL Server).
3. Execute the `schema.sql` file to generate the 13 tables.
4. Execute the `seed.sql` file to populate the database with sample data.

## Technologies Used
* SQL
* Relational Database Management System (RDBMS)
* Entity-Relationship Modeling
