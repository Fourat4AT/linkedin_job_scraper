# linkedin_job_scraper  
**Advanced LinkedIn Job Intelligence Tool**  
*AI-Powered Scraping + NLP Skill Extraction + Live Web App*

---

## Overview

A **real-time LinkedIn job scraper** that extracts, analyzes, and exports job listings with **AI-detected technical skills**.

**Key Features:**
- **AI Skill Detection** using Flair NLP (`ner-skill` model)
- **Live Web Interface** built with Gradio
- **Multi-filter Search**: City, Country, Position, Work Type, Experience Level, Time Posted
- **Live Table Updates** during scraping
- **One-Click CSV Export**
- **Stop Anytime** with instant thread termination



## Features in Detail

| Feature | Description |
|--------|-------------|
| **AI Skill Extraction** | Uses `flair-ner-skill` model to detect skills like `Python`, `AWS`, `Docker`, `TensorFlow` from job descriptions |
| **Live Scraping** | Background threading + `yield` updates Gradio table in real time |
| **Smart Filters** | Combines location, position, work type, experience, and recency |
| **Robust Error Handling** | Retry logic, timeouts, fallbacks on failed requests |
| **CSV Export** | Saves full dataset with one click to `saved_jobs/` |
| **Stop Control** | Immediate stop via `threading.Event()` |

---

## Tech Stack

```text
Python 3.8+
├── requests
├── BeautifulSoup4
├── pandas
├── gradio
├── flair (NLP)
├── threading
└── urllib3
