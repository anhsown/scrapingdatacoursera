# 📊 Coursera Course & Review Data Pipeline

## 📌 Overview
This project builds an end-to-end data pipeline to collect, process, and analyze course information and user reviews from Coursera. The system scrapes over **1,000 courses** and **140,000+ reviews**, transforming raw web data into structured datasets for further analysis and machine learning applications.

---

## 🚀 Objectives
- Crawl course metadata from Coursera
- Extract and filter course review links
- Scrape detailed user reviews
- Store and process data into structured formats (JSON, CSV)
- Prepare dataset for Data Science / NLP tasks

---

## 🧱 Project Structure
├── data/
│ ├── coursera_full_sorted.csv
│ ├── review_full.csv
│
├── crawl_courses.py # Crawl course metadata
├── crawl_reviews.py # Crawl course reviews
├── utils.py # Helper functions (read/write files)
├── README.md
