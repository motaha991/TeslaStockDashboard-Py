# Tesla Stock Price and Revenue Dashboard

This project builds a dashboard that visualizes Tesla's historical stock price and revenue trends. The data is fetched from multiple sources including Yahoo Finance and a provided revenue dataset. The project uses Python with various libraries to scrape, clean, and visualize the data in an interactive format.

## Project Overview

The main focus of this project is to:

- **Fetch Tesla stock data**: The stock data is fetched using the `yfinance` library, retrieving Tesla's historical stock prices.
- **Scrape Tesla's revenue data**: Revenue data is scraped from an external website using the `BeautifulSoup` library for web scraping.
- **Data cleaning**: The scraped revenue data is cleaned and formatted for visualization.
- **Visualization**: An interactive dashboard is created using `plotly` to visualize both Tesla's stock price and revenue over time.

## Libraries and Tools Used

- **pandas**: For data manipulation and analysis.
- **matplotlib**: For basic plotting.
- **yfinance**: To fetch Tesla's stock market data.
- **requests**: To download the HTML page containing Tesla's revenue data.
- **BeautifulSoup**: For web scraping and extracting revenue data.
- **plotly**: To create interactive graphs for stock prices and revenue.
- **plotly.subplots**: For plotting subplots to display stock prices and revenue on the same dashboard.

## Data Sources

- **Tesla Stock Data**: Fetched from [Yahoo Finance](https://finance.yahoo.com/).
- **Tesla Revenue Data**: Scraped from [this revenue data source](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-PY0220EN-SkillsNetwork/labs/project/revenue.htm).

## How It Works

1. **Stock Data**: The `yfinance` library is used to pull the complete historical stock data for Tesla. The data is then reset and processed for visualization.
2. **Revenue Data**: The Tesla revenue data is scraped using the `BeautifulSoup` library. The data is cleaned, removing extra characters (e.g., `$` and `,`), and converted to a float data type for analysis.
3. **Interactive Visualization**: The `plotly` library is used to create a dashboard with two interactive plots:
    - Tesla's historical stock price.
    - Tesla's revenue over time.
    The dashboard allows for exploring data across different time ranges.

## Sample Dashboard

The dashboard consists of two interactive plots:

1. **Historical Share Price**
   - A plot showing Tesla's stock price over time.

2. **Historical Revenue**
   - A plot showing Tesla's revenue over time.

Both plots are interactive and share a common x-axis (date), allowing users to explore the data with ease.
