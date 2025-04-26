# Book Cover Analysis with Goodreads Data

This project enhances a dataset of bestselling book covers by scraping additional metadata from Goodreads, allowing for deeper analysis and insights into design and publishing patterns.

## Project Overview

- **Original dataset**: Contains titles, authors, cover design attributes, and visual data.
- **Goal**: To explore if certain visual characteristics correlate with publishing metrics such as rating, page count, or published year.

## Workflow
1. Data Enrichment via Web Scraping
Using BeautifulSoup and requests, we scraped 5 new fields from Goodreads:
Page_count
Rating
Genre (top 2)
Publisher
First_published

**Output**: book_covers_dataset_with_goodreads.csv

2. Exploratory Data Analysis (EDA)
Conducted in **eda_book_covers.ipynb**, this step involved:
Data cleaning and normalization (categorical unification, type formatting)
Univariate analysis (title length, price, page count, etc.)
Multivariate analysis with plots to explore

**Output**: book_covers_goodreads_after_eda.csv (cleaned and analysis-ready)

3. Inferential Statistics
Performed in **inferential_statistics_book_covers.ipynb**. Includes:
Confidence Intervals: Estimated the true average Goodreads rating for the 80 books, and for top genres individually.
Hypothesis Testing: Three hypothesis tests were conducted:
-Promoted books are more recent 
-Awarded books use shorter titles 
-Visual style depends on genre

##  Folder Structure

book_analysis_dataset/
│
├── data/
│   ├── book_covers_visual_dataset.csv                # Original
│   ├── book_covers_dataset_with_goodreads.csv        # After scraping
│   ├── book_covers_goodreads_after_eda.csv           # After cleaning
│
├── eda_book_covers.ipynb                             # Exploratory analysis
├── inferential_statistics_book_covers.ipynb          # Confidence Intervals & Hypothesis Testing
├── web_scraping_goodreads.ipynb                      # Scraping logic
├── requirements.txt                                  # All libraries used
├── README.md                                         # Documentation




## How to Run

1.Clone or download this project folder to your local machine.
2.Open your terminal or Anaconda prompt.
3.Navigate to the project folder.
4.Run the following command to install required libraries:
pip install -r requirements.txt
5.Launch Jupyter Notebook
6.Open each .ipynb file to explore the steps.


## Tools and Libraries Used

pandas>=1.5.0
numpy>=1.23.0
scipy
matplotlib>=3.7.0
seaborn>=0.12.0
requests>=2.28.0
beautifulsoup4>=4.11.0
lxml>=4.9.0

## Author
This project was developed by Patricia Gimenez
Ironhack Data Analytics Bootcamp – Project 1
