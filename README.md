# Production Data Warehouse
This project was completed for 'Company A' so as to provide near real-time data replication of the production database. This database contains data from the ERP system as well as several other smaller data sources. The initial project is limited to the ERP dataset, but was later extended to include the CRM database, internal and external ticket systems, as well as some manually maintained datasets.

## Design Decisions
This data warehouse, being used for a mixture of real-time and batch calculated, requires a system that can provide very near to real-time data, as well as the scale to handle a relatively high frequency of transactions. In order to keep the solution lightweight, Change Tracking (a Microsoft developed solution) is used to track the changes on the source database, providing a seet of records to then be applied to the data warehouse. It is both lightweight on the source and allows for the process to be run at one minute intervals. This schedule allows for near real-time replication without requiring additional software.

## ER Diagram
As is common with data modeling and warehousing preparation, an example ER diagram is provided for a selection of tables. This demonstrates the interplay between tables and more detailed data models would be available to end users and analysts inside the company. This example is limited to some common tables solely for demonstrative purposes and does not include full schemas.

## Final Project
Microsoft Word was chosen to meet project criteria and include multimedia such as graphs, tables, photos and screen captures. This project document includes some example queries and JOINS using a miniturized and demilitarized version of the data warehouse running on my local machine. In addition, there are a collection of Power BI screenshots to demonstrate how this data is used in the production realm.

## Visualization
The primary purpose for this data warehouse is reporting through Power BI. This is Company A's primary reporting tool and has seen great adoption since transitioning to this data warehouse. Some example reports are contained in the project document, but there are now over 50 active reports and more in development.