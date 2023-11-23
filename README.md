# University Smart Card System

An integrated database system for IIIT Delhi college for Information Integration and Application Course (CSE656)

## About

The project involves developing and deploying an Integrated Smart Card System for university students of IIIT-Delhi. This system is engineered to streamline essential campus functions through smart card technology. Its central objective is to furnish students with identity verification, hostel, mess and campus services into an integrated student card.

## Use Cases

1. Access Control: The smart card system orchestrates secure access to university premises, including academic buildings, hostels, and labs, ensuring operational efficiency  
2. Mess Database Integration: The system integrates seamlessly with university mess facilities, allowing students to track meal selections and manage account balances.  
3. Hostel Database Integration: The smart-card system integrates the hostel database, enabling hostel check-in/check-out processes and hostel services, thus optimising hostel administration and improving student security.  
4. Sports Facilities Integration: The system facilitates real-time management and monitoring of student access to specific sports facilities within the campus sports block, ensuring efficient utilisation of resources.

## Databases

There are in total 5 Databases we wish to integrate, MessDB, HostelDB, SportDB, AccessDB and AdminDB. In total, all these databases have 14 tables combined

## Information Integration

We have performed necessary integrations needed on the data such as Schema Matching/Mapping, Entity Matching/Mapping, Data Warehousing, Materialization and ETL Tools.

## Application

Once we are ready with the data, we store it all in UniDB which allows use to perform the following applications
1. Financial Management Analytics - Displays all the financial transactions by the student across the university systems and services  
2. Mess Meal Tracking - Displays comprehensive data about student's diet and mess usage
3. Sports Inventory Management - Displays the sports equipment usage for each student for the Administration  
4. Sports Facilities Usage - Displays all the sports facilities usage for the Administration  
5. Student Access Tracking - Tracks all the student entry/exit in the Campus and buildings

## Code

1. `Data` Repository - Contains all the initial schemas as is obtained from the university  
2. `.env` - Environment variables for database connection
3. `application.py` - CLI Application for the entire project
4. `data-gen.py` - Generates CSVs for `Data` repository
5. `data-insert.py` - Adds CSV data to Local Databases
6. `extract.py` - Extracts data from Local Databases
7. `transform.py` - Converts all the data to the right format and implements a lot of integrations needed
8. `load.py` - Loads the data back to UniDB
9. `main.py` - Performs ETL
10. `run_main.sh` - Meant to periodically run ETL files
11. `data_sources_config.json` - Configures the entire schema structures for application use

## How to Use

1. Modify `.env` files accordingly, the current `.env` may not work all the time
2. Run `python application.py`
3. Enter settings
4. Run Data-Gen and Data-Insert
5. Run ETL
6. Application is ready for use

## Collaborators

Dhvanil Seth, Aajay Devaraj, Vishwesh Vhavle
