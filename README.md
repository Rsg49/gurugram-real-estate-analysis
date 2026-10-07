# 🏠 Gurugram Real Estate Analysis

## 📌 Project Overview

This project analyzes a **Gurugram real estate dataset using Python** to understand property prices, localities, BHK configurations, property types, builders, RERA approval, and the relationship between property area and price.

The project focuses on **data cleaning, exploratory data analysis (EDA), and data visualization** using Python libraries such as Pandas, Matplotlib, and Seaborn.

---

## 🎯 Project Objectives

The main objectives of this project are:

- Clean and prepare the raw real estate dataset.
- Identify the most expensive property in the dataset.
- Find localities with the highest average property prices.
- Identify localities with the highest average price per square foot.
- Compare ready-to-move and under-construction properties.
- Compare RERA-approved and non-RERA-approved properties.
- Analyze property prices based on BHK configuration.
- Identify the most expensive property types.
- Find the top 5 builders based on average price per square foot.
- Analyze the relationship between property area and price per square foot.


## 🛠️ Technologies Used

- **Python**
- **Pandas** – Data cleaning and data analysis
- **Matplotlib** – Visualization
- **Seaborn** – Data visualization
- **CSV** – Dataset format

---

## 📂 Dataset

The project uses a CSV dataset containing information about properties in Gurugram.

### Important Columns

| Column | Description |
|---|---|
| `price` | Property price |
| `area` | Property area |
| `rate_per_sqft` | Price per square foot |
| `locality` | Property locality |
| `socity` | Society/project name |
| `bhk_count` | Number of BHKs |
| `flat_type` | Type of property |
| `status` | Property construction/possession status |
| `rera_approval` | RERA approval status |
| `company_name` | Builder/company name |

---

## 🧹 Data Cleaning

Before performing the analysis, the dataset was cleaned using Pandas.

### Cleaning steps performed:

- Removed extra spaces from column names.
- Converted column names to lowercase.
- Replaced spaces in column names with underscores.
- Removed duplicate records.
- Removed commas from numerical values.
- Converted `price` into numeric format.
- Converted `area` into integer format.
- Converted `rate_per_sqft` into integer format.
- Standardized the `status` column.
- Standardized the `flat_type` column.
- Converted RERA approval values into Boolean values (`True` / `False`).

---

## 📊 Exploratory Data Analysis

The project answers the following real-world questions:

### 1. What is the costliest property?

The project identifies the property with the maximum price and displays its:

- BHK configuration
- Locality
- Price
- Society name

---

### 2. Which locality has the highest average property price?

Properties are grouped according to locality, and the **average property price** is calculated for each locality.

The locality with the highest average price is then identified.

---

### 3. Which locality has the highest average price per square foot?

The project calculates the average `rate_per_sqft` for each locality and identifies the locality with the highest average rate.

---

### 4. Do ready-to-move properties cost more than under-construction properties?

The average price of:

- Ready-to-move properties
- Under-construction properties

is calculated and compared.

This helps understand whether property status is associated with differences in average prices.

---

### 5. Do RERA-approved properties have a higher average price?

The project compares the average price of:

- RERA-approved properties
- Non-RERA-approved properties

This helps analyze whether RERA approval is associated with a higher average property price.

---

### 6. How does property area relate to price?

A scatter plot can be used to visualize the relationship between property area and total property price.

```python
sns.scatterplot(data=df, x='area', y='price')
plt.show()
```

### 7. Which BHK configuration has the highest average rate per square foot?

Properties are grouped by BHK configuration and their average price per square foot is calculated.

The BHK configuration with the highest average rate is identified.

---

### 8. Which property type has the highest average rate per square foot?

Properties are grouped by `flat_type` and compared using their average `rate_per_sqft`.

---

### 9. Which builders have the highest average price per square foot?

The project identifies the **top 5 builders** based on their average price per square foot.

The analysis uses:

- Grouping by builder
- Average rate calculation
- Sorting in descending order
- Selecting the top 5 builders

---

### 10. Are larger properties more expensive per square foot?

A scatter plot is created using:

- **X-axis:** Property Area
- **Y-axis:** Rate per Square Foot

```python
sns.scatterplot(data=df, x='area', y='rate_per_sqft')
plt.show()
```

This visualization helps analyze the relationship between property size and price per square foot.

---

## 📈 Visualizations

The project uses **Seaborn** and **Matplotlib** for data visualization.

### Area vs Price

This scatter plot shows the relationship between property area and total property price.

### Area vs Rate per Square Foot

This scatter plot helps analyze whether property size is related to the price per square foot.

---

## 🔍 Key Analysis Techniques

The project demonstrates the use of:

- Data Cleaning
- Data Preprocessing
- Exploratory Data Analysis (EDA)
- Filtering
- `groupby()`
- `mean()`
- `idxmax()`
- `sort_values()`
- `head()`
- Conditional statements
- Data Visualization
- Scatter Plots

---

## 🚀 How to Run the Project

### 1. Clone the repository

```bash
git clone YOUR_GITHUB_REPOSITORY_LINK
```

### 2. Open the project folder

```bash
cd Gurugram-Real-Estate-Analysis
```

### 3. Install required libraries

```bash
pip install pandas matplotlib seaborn
```

### 4. Make sure the CSV dataset is in the project folder

The Python program reads:

```text
data of gurugram real Estate.csv
```

### 5. Run the Python program

```bash
python gurugram_real_estate_analysis.py
```

---

## 📁 Project Structure

```text
Gurugram-Real-Estate-Analysis/
│
├── data of gurugram real Estate.csv
├── gurugram_real_estate_analysis.py
└── README.md



## 💡 Skills Demonstrated

Through this project, I demonstrated practical knowledge of:

- Python
- Pandas
- Data Cleaning
- Data Preprocessing
- Exploratory Data Analysis
- Data Aggregation
- Data Filtering
- Data Visualization
- Matplotlib
- Seaborn
- Basic Business/Data Analysis


## 🔮 Future Improvements

In the future, this project can be extended by:

- Creating an interactive dashboard using Power BI.
- Performing more detailed statistical analysis.
- Adding additional visualizations.
- Performing correlation analysis.
- Building a property price prediction model using Machine Learning.
- Using SQL for more advanced data querying.


## 👨‍💻 Author

**Rahul Singh Gaira**

