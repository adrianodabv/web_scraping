# Wikipedia Scraping Project: Largest Companies in Brazil

This project scrapes data from Wikipedia to retrieve a list of the largest companies in Brazil and exports it to a CSV file for further analysis. The project demonstrates skills in web scraping, data extraction, and data handling with Python.

## Project Overview
This script scrapes information from the Wikipedia page listing the largest companies in Brazil, gathering the data into a structured table format. It then exports the data to a CSV file, making it available for future analysis and reporting. This project is part of a portfolio highlighting data extraction and web scraping capabilities, and it can be extended to explore additional data points or to build a database of companies over time.

## Technologies Used
- **Python**: Core programming language
- **BeautifulSoup**: Library used to parse HTML and extract data from the Wikipedia page
- **Pandas**: Library for organizing and exporting the data into CSV format

## Data Source
- URL: [List of Largest Brazilian Companies on Wikipedia](https://en.wikipedia.org/wiki/List_of_largest_Brazilian_companies)
- Source Type: Public data from Wikipedia (scraped responsibly following Wikipedia's [terms of use](https://foundation.wikimedia.org/wiki/Terms_of_Use))

## Code Description
The script performs the following steps:
1. Sends an HTTP request to the Wikipedia page to retrieve HTML content.
2. Uses BeautifulSoup to parse and extract the table containing information about the largest Brazilian companies.
3. Transforms the extracted data into a `pandas` DataFrame, with column names matching the table headers.
4. Exports the DataFrame to a CSV file for easy storage and access.

### Key Code Sections
- **HTML Request**: Fetches the page content with the `requests` library.
- **HTML Parsing**: Parses HTML using `BeautifulSoup`.
- **Data Extraction**: Extracts and cleans data to populate the DataFrame.
- **CSV Export**: Saves the cleaned data to a CSV file.

## Setup Instructions
1. **Install the Required Libraries**:
   - If you haven't installed `BeautifulSoup`, `requests`, or `pandas`, install them by running:
     ```bash
     pip install beautifulsoup4 requests pandas
     ```

2. **Run the Script**:
   - Place the script in your Python environment.
   - Run the script:
     ```bash
     python your_script_name.py
     ```

3. **CSV Output**:
   - The script will generate the csv in your current directory with the data of the largest Brazilian companies.

## Sample Output
The output file will contain the following columns (subject to Wikipedia’s current structure):
- Rank
- Forbes 200 rank
- Name
- Headquarters
- Revenue
- Profit
- Assets
- Value
- Industry

## Future Enhancements
- Add error handling for network requests or changes in the webpage’s structure.
- Schedule the script to run periodically to keep the data up-to-date.

---
