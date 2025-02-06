# S&P 500 Stock Selection Based on Financial Ratios  

This script automates the selection of S&P 500 stocks based on fundamental financial metrics. It retrieves financial data, calculates key ratios, and filters stocks that exhibit consistent growth and profitability.  

## Key Features:  
1. **Retrieve S&P 500 Tickers**: Scrapes the latest S&P 500 components from Wikipedia.  
2. **Fetch Financial Statements**: Uses Yahoo Finance to obtain income statements, balance sheets, and cash flow statements.  
3. **Calculate Financial Ratios**: Computes growth metrics, valuation ratios, profitability indicators, and other key financial figures.  
4. **Filter Stocks by Sector**: Selects stocks with positive earnings, revenue, and gross profit growth across different sectors.  
5. **Export Results**: Saves the final filtered stock list to an Excel file.  

## How It Works:  
- If an existing dataset (`output.xlsx`) is found, it loads from it (it creates after the first code run); otherwise, it fetches fresh data.  
- Iterates through all S&P 500 stocks, computes financial ratios, and stores them.  
- Filters stocks that meet the growth criteria and groups them by sector.  
- Exports the filtered stock list as `Filtered Stocks.xlsx`.  

## Dependencies:  
- `pandas`  
- `yfinance`  
- `openpyxl`  

This script helps in identifying high-performing S&P 500 stocks based on fundamental analysis (which can be further personalized based on yfinance library).
