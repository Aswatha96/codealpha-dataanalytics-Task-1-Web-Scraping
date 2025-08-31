# codealpha-dataanalytics-Task-1-Web-Scraping
# Task 1 — Web Scraping (Books to Scrape)

This task scrapes product data from the demo website **Books to Scrape** (built for training/scraping practice).

## What it does
- Crawls category pages and pagination
- Extracts: Title, Price, Availability, Rating, Product URL, Image URL
- Saves results to `books.csv`

## How to run
```bash
pip install -r ../requirements.txt
python scrape_books.py
```

The script defaults to scraping a small sample (first 2 pages per category) so it runs quickly. 
Update `MAX_PAGES_PER_CATEGORY` to scrape more.

## Files generated
- `books.csv`: scraped dataset
- `logs.txt`: minimal progress log

crapes the training site Books to Scrape using requests + BeautifulSoup, paging through categories. (This site exists for learning—perfect for internships.) Output files:  books.csv — dataset with category, title, price, stock, rating, product_url, image_url  logs.txt — crawl log
