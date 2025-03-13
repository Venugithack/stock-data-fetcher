# Market Data Fetcher

## Overview
This Python script fetches stock market data from Yahoo Finance (`yfinance`), processes the data, and generates a structured PDF report using the `fpdf` library.

## Features
- Retrieves **Last Traded Price (LTP)**, **Change**, and **Change%** for global indices, commodities, and major currency pairs.
- Supports multiple market categories including **North American, European, Asian-Pacific Markets**, Commodities, Currencies, and Indian markets.
- Generates a **PDF report** with formatted market data.

## Requirements
Ensure you have the required dependencies installed before running the script:
```sh
pip install yfinance fpdf
```

## Usage
1. **Run the script:**
```sh
python app.py
```
2. The script fetches the latest stock data and generates a **market_report.pdf**.
3. The report includes key financial indicators for different markets.

## How It Works
1. **Fetch Market Data:**
   - The `fetch_ticker_data()` function retrieves stock data from Yahoo Finance.
   - The `fetch_market_data()` function iterates over different categories of tickers and fetches data accordingly.
2. **Generate PDF Report:**
   - The `generate_pdf_report()` function formats and saves the market data as a PDF file.
   
## Output
- The script creates a `market_report.pdf` file that contains structured financial data categorized by market type.

## Example
Here’s an example output format in the PDF:
```
Global Markets
  North American Markets
    Dow Jones (US) - LTP: 35,000, Change: +200, Change%: +0.57%
    Nasdaq Composite (US) - LTP: 14,200, Change: -50, Change%: -0.35%
```

## Author
Developed by **The Morning Post** for automated premarket report generation.

