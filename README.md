# Daraz-Product-Scraper
The Daraz Product Scraper is a web scraping tool designed to extract product information from the Daraz.lk website. This project focuses on leveraging data science techniques to collect, process, and analyze web data effectively. The tool is built using Python, Selenium, BeautifulSoup, and pandas, and it aims to demonstrate the application of data science in real-world web scraping scenarios.


## Features
- **Web Scraping with Selenium and BeautifulSoup:** Automates the process of extracting product data from dynamically loaded web pages.
- **Data Handling with pandas:** Structures the scraped data into a DataFrame for easy manipulation and analysis.
- **Headless Browser Execution:** Uses Selenium with headless Chrome to perform web scraping without a graphical user interface, making the process more efficient and suitable for deployment on servers.
- **Data Export to Excel:** Saves the collected data into an Excel file for further analysis or reporting.

## Overview

### 1. Web Scraping with Selenium:

- The project utilizes the Selenium WebDriver to automate the web browser interactions. Selenium is configured to run in headless mode using ChromeOptions, allowing the scraper to operate without displaying a browser window.
- A base URL is provided, and the script dynamically constructs URLs for multiple pages based on user input for the number of pages to scrape.
- The driver.get(url) method is used to navigate to each page, and time.sleep(3) ensures the page fully loads before proceeding. This waiting period might need adjustments based on network speed and website response times.

### 2. HTML Parsing with BeautifulSoup:

- After obtaining the HTML content of the page using Selenium, BeautifulSoup is employed to parse the HTML and extract relevant data. BeautifulSoup is a powerful library for parsing HTML and XML documents, making it ideal for web scraping tasks.
- The script searches for specific HTML elements (in this case, div elements with the class gridItem--Yd0sa) and extracts their text content. This part of the script may need customization based on the actual structure of the target website.
  
### 3. Data Handling and Export with pandas:

- The extracted data is stored in a list and then converted into a pandas DataFrame. pandas is a versatile data manipulation library, which allows for efficient handling and analysis of large datasets.
- The DataFrame is then exported to an Excel file using the to_excel method. This enables easy sharing and further analysis of the scraped data.

## Data Science Techniques and Insights
- **Automation:** The use of Selenium to automate web browsing and data extraction showcases how data scientists can automate repetitive tasks to collect large datasets efficiently.
- **Data Parsing and Extraction:** Demonstrates techniques for extracting structured data from unstructured HTML documents, a common requirement in data science projects involving web data.
- **Data Structuring:** Utilizing pandas to structure raw data into a tabular format facilitates subsequent data analysis and visualization tasks.
- **Scalability:** The script can be easily scaled to scrape more pages or different websites with minimal modifications, highlighting the flexibility and reusability of well-written code.

## How it works 

https://github.com/KavinduR0713/Daraz-Product-Scraper/assets/105490780/96486ac5-53d6-4a19-8a6e-9820739bf56f
