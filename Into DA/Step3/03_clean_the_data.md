# 🧼 03 – Clean the Data

“Data cleaning is like hygiene — not exciting, but absolutely necessary.”

Once you've collected the raw data, it’s rarely ready for analysis right away. You’ll need to clean it up to make sure your insights are accurate, meaningful, and not misleading.

---

## 🎯 Goals of Data Cleaning

- Handle missing or null values
- Fix incorrect or inconsistent formatting
- Remove duplicates or irrelevant records
- Convert data types where needed
- Identify and treat outliers
- Standardize column names & units

---

## 🧪 Common Data Issues

| Problem Type         | Example                                |
|----------------------|----------------------------------------|
| Missing values       | `NaN`, empty cells, `NULL`             |
| Inconsistent formats | `01-06-2023` vs `June 1, 2023`         |
| Duplicates           | Same row repeated twice                |
| Incorrect types      | "25" as string instead of integer      |
| Dirty text           | ` " yes "` instead of `yes`            |
| Outliers             | 999 in Age column                      |

---

## 🛠️ Tools for Cleaning

- `pandas` (Python) 🐼
- Power BI Query Editor
- OpenRefine
- Excel (for small-scale cleaning)

---

## 🔧 Key Cleaning Techniques (w/ Code in Notebook)

1. **Check and Handle Missing Values**
```python
df.isnull().sum()
df.fillna(0)          # Replace nulls
df.dropna()           # Drop rows with nulls
```

2. **Removing duplicates**
```python
df.drop_duplicates(inplace=True)
```
3. **Fix Column Formats**

```python

df['date'] = pd.to_datetime(df['date'])
df['amount'] = df['amount'].astype(float)
```
4. **Standardize Text**

```python

df['gender'] = df['gender'].str.strip().str.lower()
```
5. **Detect Outliers**

```python
df[df['salary'] > df['salary'].quantile(0.99)]
```
6. **Rename Columns for Clarity**

```python
df.rename(columns={'CustID': 'Customer_ID'}, inplace=True)
```


📁 [dirty_data.csv](./dirty_data.csv)  
📓 [clean_data_demo.ipynb](./clean_data_demo.ipynb)
