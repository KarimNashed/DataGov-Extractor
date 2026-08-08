Automated Web Scraper & Data Aggregation Platform

Project Overview
This project is an end-to-end data pipeline that scrapes, stores, and visualizes government dataset metadata. It features an automated web scraper built with Python that extracts dataset information from catalog.data.gov, a structured MySQL database for robust data storage, and an interactive Streamlit dashboard for data analytics and user tracking.

Key Features
* Automated Data Extraction: Uses requests and BeautifulSoup to scrape 100 pages of datasets from Data.gov, extracting metadata such as tags, formats, URLs, organizational info, and licenses.
* Relational Database Architecture: Implements a MySQL database (hosted on TiDB Serverless) with normalized tables for Organizations, Datasets, Files, Tags, AppUsers, and UsageRecords.  
* Interactive Analytics Dashboard: A Streamlit frontend that provides 11 distinct functionalities, including
	* User registration and dataset usage tracking.
	* Dataset filtering by Organization Type, Format, and Tag.
	* Aggregated statistics (e.g., Top 5 Contributing Orgs, Most Used Datasets, Top 10 Tags per Project Type).

Technologies Used
* Language: PythonWeb Scraping: BeautifulSoup4, Requests
* Database: MySQL, mysql-connector-python, TiDB Cloud  Frontend: Streamlit  

Execution Instructions
To run the analytics dashboard and web scraper locally, follow these steps:

1. Open your Mac Terminal or Windows Command Prompt.
2. Navigate to the project root folder containing app.py.
3. Create a virtual environment by running: python3 -m venv venv
4. Activate the virtual environment:
	* On Mac/Linux: source venv/bin/activate
	* On Windows: venv\Scripts\activate
5. Install the required Python libraries by running: pip3 install streamlit mysql-connector-python requests beautifulsoup4
6. Execute the application by running: streamlit run app.py