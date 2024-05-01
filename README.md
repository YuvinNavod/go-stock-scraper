# Go Stock Scraper

## Overview

Go Stock Scraper is a lightweight Go application designed to scrape stock data from various sources on the web. It leverages the power and simplicity of the Go programming language along with the `github.com/gocolly/colly` package for web scraping and `encoding/csv` for writing data to CSV files.

## Features

- Scrapes stock data including company name, price, and change.
- Supports multiple stock tickers.
- Outputs data to a CSV file for easy analysis.

## Installation

To use Go Stock Scraper, ensure you have Go installed on your system. Then, you can clone the repository:

```
git clone https://github.com/yourusername/go-stock-scraper.git
```

## Usage

1. Navigate to the project directory.
2. Run the following command to build and execute the program:

```
go run main.go
```

3. Once the program finishes execution, you will find a file named `stocks.csv` in the project directory containing the scraped stock data.

## Configuration

You can modify the list of stock tickers in the `main` function of `main.go` to scrape data for different stocks:

```go
ticker := []string{
    "MSFT",
    "AAPL",
    // Add more tickers as needed
}
```

## Dependencies

This project depends on the following Go packages:
- `github.com/gocolly/colly`: For web scraping.
- `encoding/csv`: For writing data to CSV files.

You can install these dependencies using Go modules:

```
go get -u github.com/gocolly/colly
```
