# ElectricityBillingSystem-Project

##Overview
The project is a MySQL database for an electricity billing management system. It involves several interconnected tables that store information about customers, their accounts, billing details, administrative data, electricity boards, invoices, and tariff plans. Below is a brief description of each table and its purpose:
#Tables
1.*account*: Stores information about customer accounts, including account IDs, customer IDs, account numbers, and account names. This table references the customer table for customer information.

2.*admin*: Contains data about administrators, including admin IDs, names, and associated customer IDs. It also references the customer table.

3.*billing*: Keeps track of billing details, including meter numbers, account IDs, customer IDs, monthly units consumed, amount per unit, and total amount. It references both the account and customer tables.

4.*customer*: Contains detailed information about customers, including customer IDs, names, addresses, states, cities, and pincodes. This table is referenced by multiple other tables.

5.*elec_board*: Stores information about different electricity boards, including board IDs and board names.

6.*invoice*: Contains invoice details, including invoice IDs, electricity board IDs, account numbers, tariff IDs, reading dates, and meter numbers. This table references the elec_board, tariff, and billing tables.

7.*tariff*: Stores information about different tariff plans, including tariff IDs and tariff types.The database structure supports efficient management of electricity billing and customer information, ensuring referential integrity through foreign key constraints. 

#Data
The script also includes sample data for each table, providing a realistic representation of the database's functionality. 

## Usage
To use this SQL script, execute it against your preferred SQL database management system. Make sure to adjust any table or column names as needed to fit your specific use case.

## Contributors
- Rujina Akhther (222-125-227)
- Sumaiya Begum (222-115-216)

## Queries
The script concludes with a sample query that retrieves billing information along with the associated customer names.







