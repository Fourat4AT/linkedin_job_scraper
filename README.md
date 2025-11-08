# linkedin_job_scraper
Advanced LinkedIn scraping and job data extraction using Python + BeautifulSoup

## Overview
This project is a Python-based web scraper that extracts job listings from LinkedIn. It collects information such as:

- Job Title
- Company
- Location
- Job Link
- Description
- Skills detected from the description
- Work Type
- Experience Level
- Date Scraped

The scraper uses `requests` and `BeautifulSoup` to parse LinkedIn job postings and `Gradio` for a user-friendly web interface.

---

## Features
- Filter jobs by **location**, **position**, **work type**, **experience level**, and **posting date**.
- Displays scraped job data in an interactive table.
- Export results to CSV.
- Stop scraping at any time using the interface.

---

## Requirements
- Python 3.8+
- Libraries:  
  ```bash
  pip install requests beautifulsoup4 pandas gradio
