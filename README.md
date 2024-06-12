Data Munging with Python

This repository contains Python code for data munging, specifically focused on populating a SQLite database with data from CSV files. This process involves extracting, transforming, and loading data into a structured database format.

Prerequisites
Python 3.x
SQLite3
Setup
Clone or download the repository.
Ensure Python and SQLite3 are installed on your system.
Usage
DatabaseConnector Class: This class provides methods to interact with the SQLite database.

__init__(self, database_file): Initializes the database connection.
populate(self, folder): Populates the database with data from CSV files in the specified folder.
populate_shipping_data_1(self, reader_0): Populates the shipping data from the first CSV file.
populate_shipping_data_2(self, reader_1, reader_2): Populates the shipping data from the second and third CSV files.
insert_product(self, product_name): Inserts product data into the database.
insert_shipment(self, product_name, product_quantity, origin, destination): Inserts shipment data into the database.
close(self): Closes the database connection.
Main Script:

The main script creates an instance of the DatabaseConnector class, populates the database with data from CSV files in the specified folder, and then closes the database connection.
Running the Script:

Modify the DatabaseConnector initialization to specify the path to your SQLite database file.
Ensure the CSV files containing the data are placed in the specified folder.
Run the script using Python: python script.py


Note
Customize the script according to your specific data requirements and database schema.
Ensure CSV files are formatted correctly and contain the required data columns.
This script provides a basic framework for data munging with Python. Modify and expand it as needed for your projects.
License
This code is provided under the MIT License. Feel free to use, modify, and distribute it as per the terms of the license.
