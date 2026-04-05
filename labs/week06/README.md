### **Lab 06: Web Scraping and SQLite Data Pipeline**



In this lab, we learned how to collect, store, and analyze web data using Python and SQLite. First, we scraped quotes and authors from multiple pages of the website Quotes to Scrape and stored them in a list. Next, we created a SQLite database quotes.db with a table for storing the quotes and inserted all collected data safely using parameterized queries. We then performed database operations such as reading all quotes, filtering by author, counting quotes per author, updating author names to uppercase, and deleting short quotes. Finally, we combined scraping and storage into a mini data pipeline that produced a summary report of total quotes, unique authors, and the author with the most quotes. We also practiced ethical scraping by checking the website’s robots.txt file to respect pages that should not be crawled.



#### How Data Was Scraped:

Data was collected from Quotes to Scrape, a practice website for learning web scraping.

* The Python requests library downloaded the HTML of the webpages.
* BeautifulSoup parsed the HTML to extract quote text and author names.
* Multiple pages (page 1–3) were scraped to collect more quotes.
* All data was stored in a list of dictionaries before inserting into the database.



#### How the SQLite Database Was Structured:

* Database file: quotes.db
* Table: quotes
* Columns:

  * id (INTEGER PRIMARY KEY) – unique ID for each quote
  * quote (TEXT) – text of the quote
  * author (TEXT) – name of the author
* Scraped quotes were inserted using parameterized queries for safe and reliable storage.



#### One Ethical Concern Related to Scraping:

Before scraping a website, it is important to check its robots.txt file.

* The file indicates which pages or directories bots are allowed or not allowed to crawl.
* Respecting robots.txt ensures ethical scraping and prevents overloading the website server.

