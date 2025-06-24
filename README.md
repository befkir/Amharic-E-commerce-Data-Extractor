# 🛒 Amharic E-commerce Data Extractor

This project is a web scraping tool designed to extract product information from Amharic-language e-commerce websites. It supports data collection from multiple Ethiopian online shopping platforms and saves the results into structured CSV files for analysis, search indexing, or machine learning tasks.

## 📌 Features

✅ Scrapes product titles, prices, categories, descriptions, and links

✅ Designed for Amharic-language e-commerce content

✅ Outputs clean, structured CSV files

✅ Modular design for easily adding new websites

✅ Handles different site structures and pagination

✅ Includes error handling and retry logic

## 🏗️ Tech Stack

Python 3.x

requests

BeautifulSoup

pandas

lxml

## 📂 Folder Structure

graphql

```
Amharic-E-commerce-Data-Extractor/
│
├── scrapers/
│   ├── addishiwot.py        # Scraper for Addishiwot website
│   ├── zmall.py             # Scraper for Z-Mall website
│   └── ...                  # Additional scrapers can be added here
│
├── outputs/
│   └── *.csv                # CSV files containing scraped data
│
├── utils/
│   └── helpers.py           # Shared helper functions (e.g., cleaning text)
│
├── main.py                  # Entry point to run all scrapers
├── requirements.txt         # Required Python packages
└── README.md                # Project documentation
```

## 🚀 Getting Started

1. Clone the Repository

```
git clone https://github.com/befkir/Amharic-E-commerce-Data-Extractor
cd Amharic-E-commerce-Data-Extractor
```

2. Set Up Virtual Environment (Recommended)

```
python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate
```

3. Install Dependencies

```
pip install -r requirements.txt
```

4. Run the Scraper

```
python3 main.py
```

Scraped data will be saved in the outputs/ directory.

## 🧩 Adding New Websites

To add a new e-commerce website:

Create a new file in the scrapers/ directory (e.g., myecommerce.py)

Write a scraping function that returns a list of product dictionaries

Import and call that function from main.py

📊 Output Format
Each row in the CSV includes:

Title Price Category Description Link

## 🛠️ Known Limitations

Some sites may block bots; using headers or delays might be needed

Does not yet support dynamic (JavaScript-rendered) content

No database support (yet)—currently CSV only

## 🤝 Contributing

Pull requests are welcome! If you'd like to contribute:

Fork the repository

Create a feature branch

Write clear code with comments

Submit a PR with a brief description
