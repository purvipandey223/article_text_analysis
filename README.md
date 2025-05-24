# Web Scraping and NLP Project: Article Analysis

## 📌 Project Description

This project focuses on automating the extraction and analysis of web-based articles. The aim is to scrape article content from a list of provided URLs and apply Natural Language Processing (NLP) techniques to derive various linguistic and readability insights. This includes sentiment scores, complexity metrics, word-level statistics, and more.

## 🎯 Problem Statement

Given a list of URLs pointing to blog or news articles, the task is to:

- Extract the article **title** and **main content**, excluding unwanted sections like headers, footers, ads, etc.
- Perform **text analysis** using NLP techniques to compute a set of predefined metrics.
- Output the cleaned text and computed variables in structured formats for reporting or further use.

## 🧰 Tools and Technologies Used

- **Python** 🐍
- **BeautifulSoup** & **requests** – For web scraping
- **NLTK**, **TextBlob** – For NLP and sentiment analysis
- **Pandas**, **NumPy** – For data manipulation
- **OpenPyXL** – For Excel file operations
- **Regex** – For pattern-based text cleaning


## Structure
article-text-analysis/
│
├── Input.xlsx
├── Output.xlsx
├── Output Data Structure.xlsx
├── article_text_analysis.ipynb
├── requirements.txt
├── README.md
├── Text Analysis.docx
├── Personal_Objective.docx
│
├── MasterDictionary/
│   └── ... (word lists)
│
└── StopWords/
    └── ... (custom stopword files)


## ✅ Steps to Execute

1. **Load Input URLs**  
   Read the URLs from the provided Excel file (`Input.xlsx`).

2. **Web Scraping**  
   Use BeautifulSoup and `requests` to fetch and clean the HTML content, retaining only the relevant article text.

3. **Save Cleaned Texts**  
   Store each article in a `.txt` file using its `URL_ID`.

4. **Text Analysis**  
   Apply NLP to calculate:
   - Positive and Negative Scores
   - Polarity and Subjectivity
   - Readability metrics (Fog Index, Complex Word %, Avg Sentence Length)
   - Word and syllable-level metrics

5. **Export Results**  
   Save the output in a structured Excel or CSV format, following the format in `Output Data Structure.xlsx`.


## 🚀 How to Run

1. Install dependencies:  
   ```bash
   pip install -r requirements.txt
