# AgroFarm - Exchange Rate Data Extraction and Database Integration
This repository contains a Python script for extracting exchange rate data from the ExchangeRate-API and loading it into a PostgreSQL database. The script fetches exchange rates for a base currency (NGN) against multiple currencies, processes the data, and stores it in a structured database table.

## Overview
The script performs the following tasks:

1. API Data Extraction:
    - Fetches exchange rates for NGN against currencies listed in a CSV file (currencies.csv).
    - Handles API responses and extracts relevant data (e.g., conversion rates, timestamps).

2. Data Processing:
    - Organizes the extracted data into a structured DataFrame.
    - Includes metadata such as Rate_ID, Rate_Date, Base_Currency, and Comment.

3. Database Integration:
    - Connects to a PostgreSQL database using credentials from an environment file (exch_rt.env).
    - Defines a table schema with appropriate data types.
    - Loads the processed exchange rate data into the database.

### Key Features
- API Integration: Fetches real-time exchange rate data from the ExchangeRate-API.

- Data Processing: Structures raw API responses into a clean DataFrame.

- Database Loading: Automates data loading into a PostgreSQL database.

### Repository Contents
+ Script: The main Python script for data extraction and database integration.
+ Currency List: currencies.csv containing the list of currencies to fetch exchange rates for.

### Prerequisites
+ Python 3.x
+ Libraries: requests, pandas, sqlalchemy, python-dotenv
+ DB: PostgreSQL database.
+ API key from ExchangeRate-API.

**_For any questions or issues, please open an issue in the repository. Contributions are welcome! Thank you!!!_**
