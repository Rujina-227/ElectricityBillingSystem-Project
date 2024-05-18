# ElectricityBillingSystem-Project

The project is a MySQL database for an electricity billing management system. It involves several interconnected tables that store information about customers, their accounts, billing details, administrative data, electricity boards, invoices, and tariff plans. Below is a brief description of each table and its purpose:

1.account: Stores information about customer accounts, including account IDs, customer IDs, account numbers, and account names. This table references the customer table for customer information.

2.admin: Contains data about administrators, including admin IDs, names, and associated customer IDs. It also references the customer table.

3.billing: Keeps track of billing details, including meter numbers, account IDs, customer IDs, monthly units consumed, amount per unit, and total amount. It references both the account and customer tables.

4.customer: Contains detailed information about customers, including customer IDs, names, addresses, states, cities, and pincodes. This table is referenced by multiple other tables.

5.elec_board: Stores information about different electricity boards, including board IDs and board names.

6.invoice: Contains invoice details, including invoice IDs, electricity board IDs, account numbers, tariff IDs, reading dates, and meter numbers. This table references the elec_board, tariff, and billing tables.

7.tariff: Stores information about different tariff plans, including tariff IDs and tariff types.The database structure supports efficient management of electricity billing and customer information, ensuring referential integrity through foreign key constraints. 

The data inserted into these tables includes sample records for accounts, administrators, billing details, customers, electricity boards, invoices, and tariffs.The database also includes settings and commands to ensure proper configuration and optimization, such as disabling and enabling keys during data insertion to improve performance and maintaining character set consistency. The final SQL statement selects billing information along with customer names, demonstrating a typical query to retrieve relevant data from the database.
