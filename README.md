# SpaceX Falcon 9 and Falcon Heavy Launch Data Scraper
This project scrapes and processes data on SpaceX Falcon 9 and Falcon Heavy launches from a Wikipedia page using Python's requests and BeautifulSoup libraries. The extracted data is saved into a Pandas DataFrame for further analysis.

## Project Overview
The code in this repository performs the following tasks:

Web Scraping: Uses requests to retrieve the Wikipedia page that lists Falcon 9 and Falcon Heavy launches.
HTML Parsing: Utilizes BeautifulSoup to parse the HTML tables and extract relevant information such as flight number, date, launch site, payload, and more.
Data Cleaning: Processes the extracted data by removing unwanted elements and normalizing values such as payload mass.
Data Storage: Stores the processed data into a Pandas DataFrame for analysis or exporting to CSV.
## Files
spacex_launch_scraper.py: The main Python script that performs web scraping and data extraction.
requirements.txt: List of required Python libraries.
Features Extracted
Flight Number
Date and Time
Version of the Booster
Launch Site
Payload Name
Payload Mass (kg)
Orbit
Customer
Launch Outcome
Booster Landing Status
## How to Run
Install the required packages:
bash
Copy code
pip install -r requirements.txt
Run the script:
bash
Copy code
python spacex_launch_scraper.py
The extracted data will be printed and stored in a Pandas DataFrame.
## Dependencies
requests
beautifulsoup4
pandas
re
unicodedata
## Example Output
The output of the script is a table-like DataFrame that looks like:

Flight No.	Date	Time	Version Booster	Launch Site	Payload	Payload Mass	Orbit	Customer	Launch Outcome	Booster Landing
1	24 May 2012	07:44	Falcon 9 v1.0	Cape Canaveral	Dragon C2+	525kg	LEO	NASA	Success	Yes
