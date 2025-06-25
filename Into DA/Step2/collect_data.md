# 📦 02 – Collect the Data

Data is the foundation of all analysis.  
Before you can clean, analyze, or visualize anything, you need to **collect data that actually matters**.

This module will teach you:

- 🎯 What data to collect
- 🔍 Where to find it
- 🧰 How to collect it (tools & techniques)
- ⚠️ Common challenges
- 📁 Real-world examples

---

## 🧠 1. Ask Before You Collect

Before hunting for data, ask yourself:

- ❓ What is the business problem?
- 🎯 What questions am I trying to answer?
- 🧑‍💼 Who are the stakeholders?
- 📈 What kind of analysis or model do I want to build?

👉 Example:
> If you're analyzing customer churn, do you need usage logs, demographics, purchase history?

---

## 🌍 2. Types of Data

| Type       | Example                               | Source                       |
|------------|----------------------------------------|------------------------------|
| Structured | Tables, CSV, Excel, SQL DBs            | CRMs, ERPs, Google Sheets    |
| Semi-structured | JSON, XML, logs                  | APIs, IoT Devices, Webhooks  |
| Unstructured | Text, images, audio, video         | Social media, documents      |

---

## 🔧 3. Common Data Sources

### 📄 Flat Files
- `.csv`, `.xlsx`, `.txt` files
- Found in Kaggle, open data portals, exports

### 🌐 APIs
- Fetch data using code from services like:
  - [Twitter API](https://developer.twitter.com/)
  - [OpenWeather](https://openweathermap.org/api)
  - [CoinGecko](https://www.coingecko.com/en/api)

### 🌐 Web Scraping
- Scrape data from websites using tools like:
  - BeautifulSoup
  - Scrapy
  - Selenium
- Example: Scrape job listings, stock prices, ecommerce products

### 📊 Public Datasets
- Kaggle ([kaggle.com/datasets](https://www.kaggle.com/datasets))
- Google Dataset Search
- Government portals (e.g. data.gov.in)
- World Bank, UCI ML Repository

### 🧪 Database Connections
- Pull directly from:
  - MySQL, PostgreSQL
  - MongoDB
  - Firebase
- Use Python (SQLAlchemy, PyMongo) or tools like Power BI

### 🛠️ Internal Systems
- Company databases
- Excel dashboards
- Product analytics tools like Mixpanel, GA4

---

## ⚙️ 4. Tools for Collecting Data

| Tool        | Purpose                             |
|-------------|-------------------------------------|
| `pandas`    | Read CSV, Excel, SQL, JSON          |
| `requests`  | Call APIs                           |
| `BeautifulSoup` | Web scraping HTML pages        |
| `Power BI` / `Tableau` | Connect to online sources |
| `Google Sheets API` | Live data from Sheets       |
| `SQL`       | Extract data with queries           |

---

## 🧯 5. Data Collection Challenges

- ⛔ Incomplete data (missing rows/columns)
- ⚠️ Biased sources (non-representative)
- 🚫 API limits or paywalls
- 🔐 Access issues or permissions
- 💀 Dead links or outdated datasets

👉 Always evaluate **data quality**: is it accurate, recent, complete, unbiased?

---

## 💡 6. Pro Tips for Real Ones

- 🔎 Start small — test the source first
- 🧼 Collect *only what you need* — don’t hoard
- 🧾 Document your source (URL, access date, version)
- 🔁 Automate with scripts or scheduled pulls (cron jobs, Zapier)
- 🧠 Always think ahead: Will this data need cleaning? Is it analysis-ready?

---

## 🧪 7. Practice Exercise

> ✅ Try collecting data from **at least 2 different sources**:

1. One public dataset (from Kaggle or Data.gov)
2. One scraped dataset (like IMDb movies or Flipkart prices)

Then answer:
- What’s the format?
- What are the challenges you faced?
- Is it structured/semi/unstructured?
- What would you analyze with this?

---

## 📚 Bonus: Real-World Examples

| Use Case                          | Data Source                                |
|----------------------------------|--------------------------------------------|
| Netflix Recommender              | Kaggle movie dataset                       |
| Startup Growth Dashboard         | Crunchbase API + Excel dump                |
| Weather Prediction Model         | OpenWeather API                            |
| Twitter Sentiment Analyzer       | Twitter API + BeautifulSoup                |
| Sales Analysis                   | Company CRM export (Excel/CSV)             |

---

## 🧘 Final Thought:

> “Data is not just numbers. It’s the start of a story.  
Choose your source like a writer picks a pen — wisely.” ✍️📦

---
# 📦 02 – Collect the Data

Before any magic can happen in data analysis, you need the *right* data — reliable, relevant, and ready to roll. This module helps you learn what to collect, where to find it, and how to get it like a pro analyst.

---

## 🎯 Goals of This Step

- Understand what data to collect for your problem
- Explore different data sources
- Use tools to collect and import data
- Evaluate data quality before moving ahead

---

## 🧠 1. Ask the Right Questions First

Before collecting data, clarify:
- What is the objective of the analysis?
- What business questions are you answering?
- What kind of data will help? (numeric, text, dates?)
- Who will use these insights?

> ✅ Example: Want to predict churn? You might need user demographics, purchase history, engagement data, and subscription length.

---

## 🌍 2. Types of Data Sources

| Type       | Examples                            | Format     |
|------------|-------------------------------------|------------|
| Structured | Excel, CSV, SQL Tables              | Tabular    |
| Semi-structured | JSON, XML, Logs               | Nested     |
| Unstructured | PDFs, Images, Tweets             | Raw/Text   |

---

## 🔧 3. Common Ways to Collect Data

### 📁 Flat Files (CSV, Excel, TXT)
- Best for quick analysis and manual collection
- Found on Kaggle, UCI ML repo, data.gov.in

### 🌐 APIs
- Pull real-time or historical data programmatically
- Tools: `requests`, `Postman`, `RapidAPI`
- Examples: Twitter API, CoinGecko API

### 🧼 Web Scraping
- Pull data directly from websites (public pages only)
- Tools: `BeautifulSoup`, `Selenium`, `Scrapy`
- Example: Scrape movie ratings from IMDb

### 📊 Public Datasets
- [Kaggle Datasets](https://kaggle.com/datasets)
- [Google Dataset Search](https://datasetsearch.research.google.com/)
- [data.gov.in](https://data.gov.in/)
- [UCI ML Repository](https://archive.ics.uci.edu/ml/index.php)

### 🔌 Databases
- SQL: MySQL, PostgreSQL
- NoSQL: MongoDB, Firebase
- Accessed via `pymysql`, `SQLAlchemy`, `PyMongo`

---

## 🛠️ 4. Tools to Use

| Tool          | Use Case                          |
|---------------|-----------------------------------|
| `pandas`      | Read Excel, CSV, SQL, JSON        |
| `requests`    | Call APIs                         |
| `BeautifulSoup` | Web scraping (HTML parsing)    |
| `Power BI`    | Import from APIs, Excel, SQL      |
| `Google Sheets API` | Real-time sheets data      |

---

## ⚠️ 5. Data Collection Challenges

- Missing or incomplete records
- Rate limits on APIs
- Captchas while scraping
- Outdated or inconsistent sources
- Permission/access errors
- Poorly structured files

---

## 📁 6. Sample Data Sources (see: `data_sources_list.csv`)

| Source Type      | Platform         | Format  | Link                                      |
|------------------|------------------|---------|-------------------------------------------|
| Public Dataset   | Kaggle           | CSV     | https://kaggle.com                        |
| API              | OpenWeather      | JSON    | https://openweathermap.org/api           |
| Web Scraped Data | IMDb Movies      | HTML    | https://www.imdb.com/chart/top           |
| Internal Export  | Company CRM      | Excel   | (confidential)                            |

---

## 🧪 7. Practical Exercise

> ✅ Choose 2 data sources and collect sample datasets.  
Answer these questions:

1. What format is the data in?
2. Is it structured/semi/unstructured?
3. What are the challenges you faced?
4. What insights could be extracted?

---

## 💻 8. Demo Notebook: `collect_data_demo.ipynb`

Includes:
- Reading CSV using `pandas`
- Calling a public API using `requests`
- Scraping a simple HTML table using `BeautifulSoup`
- Viewing head of DataFrame

---





---

