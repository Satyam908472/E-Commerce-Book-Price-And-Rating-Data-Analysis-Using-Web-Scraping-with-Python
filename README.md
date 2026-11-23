📚 E-Commerce Book Price Analysis | Web Scraping with Python

📌 Project Overview

This project focuses on collecting, cleaning, validating, and analyzing e-commerce product data using **Python Web Scraping** techniques.

The data is scraped from [Books to Scrape](https://books.toscrape.com/), a demo website designed for practicing web scraping.

The project uses Python libraries such as Requests, BeautifulSoup, Pandas, and Regular Expressions to extract book information from multiple pages and transform it into a structured dataset.

The final dataset is exported into a CSV file for further analysis and visualization.

🎯 Project Objectives

- Extract product information from an e-commerce website.
- Scrape data from multiple pages using pagination.
- Collect book names, prices, ratings, and availability.
- Clean and standardize the scraped dataset.
- Identify missing values and duplicate records.
- Validate data types and price/rating ranges.
- Export the cleaned dataset into CSV format.

🛠️ Technologies & Libraries Used

| Technology | Purpose |
|---|---|
| Python | Programming language |
| Requests | Sending HTTP requests to the website |
| BeautifulSoup | Extracting information from HTML |
| Pandas | Data manipulation and analysis |
| Regular Expressions (re) | Cleaning price values |
| Time | Adding delays between requests |
| URLlib | Handling and combining URLs |
| Datetime | Recording scraping timestamps |
| Jupyter Notebook | Writing and executing Python code |

🌐 Data Source

**Website:** https://books.toscrape.com/

Books to Scrape is a sample e-commerce website used for practicing web scraping.

The scraper extracts the following information:

| Column Name | Description |
|---|---|
| product_name | Name of the book |
| price_gbp | Book price in British Pounds (£) |
| rating | Customer rating (1–5) |
| availability | Product stock availability |
| category | Product category |
| product_url | Individual product page URL |
| scraped_at | Date and time when the data was scraped |

⚙️ Project Workflow

1. Web Scraping

- Sent HTTP requests using the Requests library.
- Parsed HTML content using BeautifulSoup.
- Extracted product details using CSS selectors.
- Collected data from multiple pages.
- Implemented pagination to navigate through the website.
- Used `urljoin()` to generate complete product URLs.

2. Data Collection

Collected the following product attributes:

- Product Name
- Price (GBP)
- Rating
- Availability
- Category
- Product URL
- Scraping Timestamp

3. Data Cleaning

Performed the following cleaning operations:

- Removed leading and trailing spaces from product names.
- Converted price values into numeric format.
- Converted ratings into numeric format.
- Converted scraping timestamps into datetime format.
- Standardized availability text.
- Removed duplicate product URLs.
- Checked for missing values.

4. Data Validation

Validated the dataset by checking:

- Total number of records.
- Number of columns.
- Column names and data types.
- Missing values.
- Duplicate product URLs.
- Duplicate product names.
- Invalid or missing prices.
- Ratings outside the valid range of 1 to 5.

5. Data Export

Exported the scraped dataset into a CSV file:

`ecommerce_products_full.csv`

The CSV file can be used for further analysis in Python, Excel, SQL, or Power BI.

📊 Project Results

The scraper is designed to collect data across all available pages of the website.

The project output includes:

- A structured product dataset.
- Product prices in GBP.
- Numerical customer ratings.
- Product availability information.
- Unique product URLs.
- Scraping timestamps.
- Data quality validation results.

*Note: Add your final verified dataset statistics here after executing the notebook.*

📂 Project Structure

```text
Book-Price-Analysis/
│
├── Web_Scraping.ipynb
│
├── ecommerce_products_full.csv
│
├── README.md
│
└── screenshots/
    ├── scraping_output.png
    ├── dataset_preview.png
    └── data_validation.png
```

🚀 How to Run This Project

### Step 1: Clone the Repository

```bash
git clone https://github.com/Satyam908472/Book-Price-Analysis.git
```

### Step 2: Navigate to the Project Folder

```bash
cd Book-Price-Analysis
```

### Step 3: Install Required Libraries

```bash
pip install requests pandas beautifulsoup4
```

### Step 4: Open Jupyter Notebook

```bash
jupyter notebook
```

### Step 5: Run the Notebook

Open `Web_Scraping.ipynb` and execute the cells sequentially.

After successful execution, the dataset will be saved as:

`ecommerce_products_full.csv`

💡 Key Learnings

Through this project, I gained practical experience in:

- Understanding HTML structure and CSS selectors.
- Sending HTTP requests and handling responses.
- Extracting data using BeautifulSoup.
- Implementing multi-page web scraping.
- Cleaning and transforming datasets using Pandas.
- Handling missing values and duplicate records.
- Performing data quality checks.
- Exporting structured data into CSV files.

🔮 Future Improvements

- Extract individual book categories dynamically.
- Scrape additional product details from individual product pages.
- Perform exploratory data analysis (EDA).
- Create interactive dashboards using Power BI.
- Analyze price distribution and customer ratings.
- Store scraped data in an SQLite database.
- Automate periodic data collection.

⚠️ Disclaimer

This project is developed for educational and learning purposes using the Books to Scrape demo website.

The scraping process includes a small delay between requests to avoid sending requests too frequently.

👨‍💻 Author

**Satyam Pandey**

Aspiring Data Analyst | Python | SQL | Pandas | Web Scraping | Data Visualization

GitHub: https://github.com/Satyam908472

⭐ If you find this project useful, feel free to star the repository!
