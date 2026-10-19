# Bookstore Intelligence Scraper
Web scraper for https://books.toscrape.com/ (practice sandbox) built with requests, BeautifulSoup and pandas.

**Author:** Ahmed Hassan (23i-5018) | Business Data and Text Mining

## How it works
1. `scrape_page(url)` fetches one catalogue page and extracts title, price, rating (word converted to 1-5), availability and product URL.
2. `scrape_all(pages)` loops over the pages, so the code is not repeated.
3. Results go into a pandas DataFrame and are saved to `competitor_books.csv`.
4. The script answers the business questions, solves the £100 challenge with a knapsack algorithm, and plots rating counts.

## Run it
pip install requests beautifulsoup4 pandas matplotlib numpy
python bookstore_scraper.py

## Key findings (100 books)
- Average price £34.56; 19 five-star books
- 5-star books average £30.01, cheaper than the overall average
- £100 challenge: 7 books, £98.61, total rating 31
