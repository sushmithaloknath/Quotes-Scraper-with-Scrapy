# Quotes-Scraper-with-Scrapy

This Scrapy project contains a spider named `quotes` that scrapes quotes, authors, and tags from the website [Quotes to Scrape](http://quotes.toscrape.com/). The spider automatically follows pagination links to scrape all pages.

---

## Features

- Extracts quote text, author name, and associated tags.
- Automatically navigates through all paginated pages.
- Outputs scraped data in structured formats like JSON, CSV, or XML.

---

## Requirements

- Python 3.x
- Scrapy

---

## Installation

1. Install Scrapy:
   ```bash
   pip install scrapy
2. Create a new Scrapy project (if you haven’t yet):
scrapy startproject quotes_scraper
cd quotes_scraper
3. Save the spider script (quotes_spider.py) inside the spiders directory of your Scrapy project.
   Usage
Run the spider from your project’s root directory:

scrapy crawl quotes -o quotes.json
This will scrape all quotes and save the output into quotes.json.

You can also export to other formats:

scrapy crawl quotes -o quotes.csv
scrapy crawl quotes -o quotes.xml
