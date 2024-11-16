# Web Scraping and Analysis of Flipkart Gaming Laptop Prices
This repository contains code for web scraping gaming laptop details from Flipkart and performing exploratory data analysis (EDA) on the extracted data.

## 1. Introduction
This project demonstrates web scraping using Selenium to extract information on gaming laptops from Flipkart. The extracted data is then cleaned, processed, and analyzed using pandas, NumPy, and visualization libraries like Matplotlib, Seaborn, and Plotly.

## 2. Data Acquisition (Web Scraping)
The script utilizes Selenium to navigate Flipkart's gaming laptop search results pages. It extracts the following information for each laptop:

Name: Laptop model name

Price: Price (after handling potential discounts)

Rating: Customer rating (if available)

Processor: Processor type

RAM: RAM size and type

Operating System: Operating system

Storage: Storage size and type

Display: Display size

Inclusion: Additional features (warranty, etc.)

The scraping is designed to handle multiple pages of search results.

## 3. Data Processing and Cleaning
The extracted data is organized into a Pandas DataFrame. Data cleaning includes:

Handling missing values (if any).

Converting price to numeric format.

Removing irrelevant characters from text fields.

## 4. Exploratory Data Analysis (EDA)
The EDA focuses on answering several key questions regarding gaming laptop prices and specifications:

Most/Least Expensive Laptops: Identifying the most and least expensive laptops among the top N results. (Visualized with a horizontal bar chart)

Laptop Prices by Processor: Analyzing the average price by processor type (Visualized with a bar chart).

RAM Price Analysis: Examining the average price across different RAM configurations (Visualized with a pie chart).

Common Storage/RAM Combinations: Investigating the most frequent combinations of storage and RAM sizes (Visualized with a sunburst chart).

Storage Size Price Analysis: Analyzing average price across different storage sizes (Visualized with a pie chart).

## 5. Results and Visualizations
The EDA results are presented through various visualizations, including bar charts, pie charts, and a sunburst chart. The generated charts aim to provide clear insights into the relationship between price, processor, RAM, storage, and display size of gaming laptops listed on Flipkart. These visualizations are located in the notebook.

## 6. Code Structure
The code is organized into sections for:

Importing Libraries: Imports necessary libraries like pandas, selenium, matplotlib, seaborn, and plotly.

Web Scraping: The core Selenium code for extracting data.

Data Frame Creation and Cleaning: Creates and cleans the Pandas DataFrame.

Exploratory Data Analysis: Performs EDA and generates visualizations.

## 7. Dependencies
To run this code, you will need the following Python libraries:

pandas

selenium

numpy

matplotlib

seaborn

plotly

Install using pip install pandas selenium numpy matplotlib seaborn plotly

You will also need a webdriver for your browser (e.g., ChromeDriver for Chrome). Make sure it's in your system's PATH or specify its location in the code.

## 8. How to Run
Install the required libraries (see above).

Download the ChromeDriver (or other relevant webdriver) and ensure it is in your system's PATH or adjust the webdriver path in the code.

Run the Python script. The visualizations will be displayed.

## 9. Limitations
The scraping depends on the structure of the Flipkart website. Changes to the website might break the script.

The script scrapes only a limited number of pages.

Error handling is basic; more robust error handling could be added.

This README gives a comprehensive overview of the project. Remember to always respect the website's terms of service when scraping data. Adding more sophisticated error handling and expanding the scraping to more pages would enhance the project's robustness.
