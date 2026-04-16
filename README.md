# Coursera Course & Review Data Pipeline

## Overview
This project builds an end-to-end data pipeline to collect, process, and analyze course information and user reviews from Coursera. The system scrapes over **1,000 courses** and **140,000+ reviews**, transforming raw web data into structured datasets for further analysis and machine learning applications.

---

## Objectives
- Crawl course metadata from Coursera
- Extract and filter course review links
- Scrape detailed user reviews
- Store and process data into structured formats (JSON, CSV)
- Prepare dataset for Data Science / NLP tasks

---
## Pipeline Workflow

### Step 1: Crawl Course Links
- Use Selenium to scroll and load dynamic content
- Extract course URLs using BeautifulSoup
- Save to: list_coursera_links.txt


---

### Step 2: Crawl Course Metadata
For each course:
- Organization name
- Course name
- Rating (stars)
- Number of reviews
- Level
- Learning outcomes

Output: coursera_full_sorted.csv


---

###  Step 3: Filter Review Links
- Identify courses containing "Reviews" section
- Generate review page links

 Output: list_review_links.txt
 
---

###  Step 4: Crawl Reviews
For each course:
- Reviewer name
- Review date
- Review content
- Rating stars

 Output: review_full.csv
 
---

### Step 5: Merge & Process Data
- Combine all CSV files into one dataset
- Clean and preprocess data for analysis

---

##  Dataset Summary

###  Course Dataset
- ~1,000 courses
- Features:
  - `organization_name`
  - `coursera_name`
  - `star`
  - `reviews`
  - `level`
  - `result`

---

###  Review Dataset
- ~140,804 reviews
- Features:
  - `Coursera Name`
  - `Reviewer Name`
  - `Date of Review`
  - `Review Contents`
  - `Rating star`

---

##  Data Preprocessing
- Handle missing values (`NaN`)
- Normalize text (lowercase, remove noise)
- Convert data types (ratings, dates)
- Align course names for merging datasets

---

## 📈 Potential Analysis & Applications

### Exploratory Data Analysis (EDA)
- Distribution of ratings
- Most reviewed courses
- Rating by course level

### Machine Learning / NLP
- Sentiment Analysis
- Rating prediction from text
- Keyword extraction
- Review classification

---

##  Technologies Used
- Python
- Selenium
- BeautifulSoup
- Pandas
- NumPy

---

## Limitations
- Some pages have inconsistent HTML structure
- Partial data collected due to time constraints
- Heavy reliance on XPath may break if UI changes

---

## Future Improvements
- Add retry & logging system
- Optimize crawling performance
- Use APIs if available
- Apply deep learning models (BERT for NLP)
- Deploy as a data pipeline

---

## Key Achievements
- Built a scalable web scraping pipeline
- Collected large-scale real-world dataset (140k+ reviews)
- Structured unstructured web data into usable format
- Prepared dataset for AI/Data Science tasks

---

## Project Highlights
> Built an end-to-end data pipeline to scrape and process over 140,000 course reviews and 1,000+ course metadata entries from Coursera, enabling downstream analysis and machine learning applications.


