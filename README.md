# Data-Entry-Job-Automation-Web-Scrape-Google-Form-Google-Sheet-

Automate a data-entry “job” by scraping real-estate listings from the web (e.g., Zillow-style results) and submitting each record into a Google Form, which pipes responses into a Google Sheet. This project showcases requests + BeautifulSoup for scraping and Selenium for browser automation with sensible rate-limits, retries, and selector hygiene.

# ✨ Features

Scrape listing cards → grab Address, Price, and Listing URL

Normalize data → trim spaces, unify currency, ensure absolute URLs

Automate form submissions → one response per listing (Form → Sheet)

Resilient automation → explicit waits, retries, optional headless mode

Idempotent runs → dedupe by canonical listing URL

Local snapshots → CSV export of the scraped dataset (for debugging/audits)

# 🧱 Tech Stack

Python 3.10+

requests + BeautifulSoup4 — HTML fetch & parse

Selenium 4 — form filling (uses Selenium Manager to auto-resolve drivers)

pandas — optional CSV export / quick checks

python-dotenv — optional config via .env
