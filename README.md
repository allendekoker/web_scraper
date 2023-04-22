# README for web_scraper.py

This is a Python script for web scraping that extracts all the URLs on a given webpage and writes them to a CSV file. It uses the requests and BeautifulSoup libraries for making HTTP requests and parsing HTML.

## How to use

1. Set the `url` variable to the URL of the webpage you want to scrape.
2. Run the script.
3. The script will create a CSV file named "links.csv" in the same directory as the script.
4. The CSV file will contain one column named "URL" and one row for each URL found on the webpage.

## Dependencies

This script requires the following Python libraries:

- requests
- BeautifulSoup
- csv

## How it works

1. The script makes an HTTP GET request to the specified URL using the requests library.
2. If the response status code is 200, the HTML content of the response is parsed into a BeautifulSoup object.
3. The script finds all the `<a>` tags in the parsed HTML using the `find_all` method.
4. The script writes the URLs to a CSV file using the csv library.

## Disclaimer

Please note that web scraping can be unethical or illegal if not done properly. Always respect the website's terms of service and privacy policy, and ensure that you have the necessary permissions before scraping any website.