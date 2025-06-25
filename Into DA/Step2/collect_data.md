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

