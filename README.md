# Smartwatch-Market-Analysis-EDA-Web-Scraping-
Smartwatch Market Analysis using Python, Web Scraping, Pandas, NumPy, Matplotlib, and Seaborn to analyze product prices, brands, ratings, reviews, and market trends.
# ⌚ Smartwatch Market Analysis Using Amazon.in Web Scraping

An end-to-end Data Analytics project that collects smartwatch data from **Amazon.in** using **Web Scraping**, cleans and preprocesses the data, and performs **Exploratory Data Analysis (EDA)** to uncover trends in smartwatch pricing, brands, ratings, discounts, and display sizes.

---

## 📌 Project Overview

This project demonstrates the complete data analytics workflow:

- 🌐 Web Scraping smartwatch data from Amazon.in
- 🧹 Data Cleaning & Preprocessing
- 🛠️ Feature Engineering
- 📊 Exploratory Data Analysis (EDA)
- 📈 Data Visualization
- 🧪 Outlier Testing (IQR & Z-Score)
- 💡 Business Insights

The objective is to help customers find the best value-for-money smartwatches and to help smartwatch companies understand pricing strategies, customer preferences, and the relationship between price and features.

---

## ❓ Business Problem

Customers face difficulty while purchasing smartwatches because:

- A large number of smartwatch brands and models are available online
- It is hard to identify the best value-for-money smartwatches
- It is hard to compare features such as battery life, display, health tracking, and calling options

Smartwatch companies also need insights into:

- Pricing strategies
- Customer preferences
- Popular smartwatch brands and models
- The relationship between price and features

---

## 🎯 Problem Statement

- Collect smartwatch data from online websites using web scraping to analyze prices, discounts, and features
- Clean and preprocess the data by handling missing values, removing duplicates, and treating outliers
- Perform EDA and data visualization to identify pricing patterns, popular features, and the best value-for-money smartwatches

---

## 🚀 Features

- Scrapes smartwatch listings directly from Amazon.in
- Extracts important product details such as:
  * Product Name
  * Brand
  * Display Size
  * Selling Price
  * Original Price (MRP)
  * Discount
  * Rating
  * Reviews
- Cleans inconsistent and missing values
- Engineers new features (Discount Amount, Price Category, Rating Category)
- Detects outliers using IQR and Z-Score methods
- Generates univariate, bivariate, and multivariate visualizations
- Produces business recommendations based on the analysis

---

## 📂 Project Workflow

```
Amazon.in Website
        │
        ▼
Web Scraping (Requests + BeautifulSoup)
        │
        ▼
Raw Dataset (Pandas DataFrame)
        │
        ▼
Data Cleaning & Preprocessing
        │
        ▼
Feature Engineering
        │
        ▼
Exploratory Data Analysis
        │
        ▼
Visualizations & Outlier Testing
        │
        ▼
Business Insights
```

---

## 🛠️ Technologies Used

- Python
- Requests
- BeautifulSoup
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## 🗃️ Dataset Description

The collected dataset contains **517 smartwatch records** with **8 attributes**, each describing a smartwatch listing on Amazon.in.

| Column Name | Description |
| --- | --- |
| Product_name | Name / title of the smartwatch listing |
| Brand | Brand of the smartwatch |
| Display | Display size of the watch (inches) |
| Price | Selling price of the smartwatch (₹) |
| Original_Price | Original (MRP) price before discount (₹) |
| Discount | Discount offered on the product |
| Rating | Average customer rating (out of 5) |
| Reviews | Number of customer reviews |

---

## 🧹 Data Cleaning & Preprocessing

- Checked dataset structure using `info()`, `describe()`, and `isnull()`
- Handled missing values using Mean, Median, and Mode
- Removed duplicate records
- Converted columns into proper data types (Price, Discount, Ratings, Reviews)
- Extracted important product details (Brand, Display Size, Original Price)
- Detected outliers using the IQR Method and Z-Score Method

---

## ⚙️ Feature Engineering

| New Feature | Description |
| --- | --- |
| Discount Amount | `Original Price − Selling Price`; helps identify customer savings |
| Price Category | Budget, Mid-Range, Premium, and Luxury segments |
| Rating Category | Groups smartwatches by customer rating to identify highly rated products |
| Brand | Brand names extracted from product titles for brand-wise comparison |

---

## 📊 Analysis Performed

**Univariate Analysis**
- Price Distribution
- Rating Distribution
- Top 10 Brands by Product Count
- Display Size Distribution

**Bivariate Analysis**
- Display Size vs Average Price
- Top 10 Brands by Average Price
- Price vs Rating

**Multivariate Analysis**
- Correlation Heatmap (Price, Original Price, Discount, Rating, Reviews)

---

## 📈 Visualizations

The notebook includes visualizations using Matplotlib and Seaborn such as:

- Histogram
- Bar Chart
- Count Plot
- Scatter Plot
- Correlation Heatmap

---

## 💡 Key Insights
---

* Brands: Fastrack has the most product listings, while Garmin has the highest average price.

* Ratings: Most smartwatches receive ratings around 3.9 to 4.0, indicating generally positive customer feedback.

* Display: 1.43 inches is the most common display size.

* Correlation: Original price and selling price have a positive relationship.

* Discounts: Higher discounts are generally associated with lower selling prices.

* Customer Ratings: Higher-priced smartwatches tend to have better ratings, but price alone does not guarantee customer satisfaction.
*
---

## 📁 Project Structure

```
Smartwatch-Analysis/
│
├── Smartwatch_Analysis.ipynb
├── Scraped_Smartwatch_Data.csv
├── Cleaned_Smartwatch_Data.csv
├── Smartwatch_Analysis_PPT.pptx
├── README.md
```

---

## ▶️ How to Run

1. Clone this repository

```
git clone https://github.com/krishnababuelarapu-bit/Smartwatch-Analysis.git
```

2. Install required libraries

```
pip install pandas numpy matplotlib seaborn requests beautifulsoup4
```

3. Open the notebook

```
jupyter notebook
```

4. Run all cells.

---

## ✅ Conclusion

- Successfully scraped smartwatch data from Amazon.in using Requests and BeautifulSoup
- Performed complete data cleaning and feature engineering
- Conducted detailed EDA and visualization
- Identified important pricing patterns and market trends
- Validated data quality using IQR and Z-Score outlier testing
- Generated meaningful business insights and recommendations

The project demonstrates how **Web Scraping + EDA** can help understand online smartwatch market behavior and support data-driven decision making.

---

## 🎯 Skills Demonstrated

- Web Scraping
- Data Collection
- Data Cleaning
- Data Preprocessing
- Feature Engineering
- Exploratory Data Analysis (EDA)
- Data Visualization
- Statistical Analysis
- Business Insight Generation
- Python Programming

---

## 📌 Future Improvements

- **Rating Prediction:** build a classification model to predict whether a smartwatch will be highly rated using price, brand, and discount
- **Feature Extraction:** extract details like battery life, GPS, AMOLED display, and water resistance from product titles
- **Multi-Platform Comparison:** collect data from Flipkart and other e-commerce sites to compare prices and ratings across platforms
- **Streamlit Web App:** build an interactive app to filter and compare smartwatches by budget, brand, and features

---

## 👨‍💻 Author

**Krishna Babu Elarapu**

Motivated and analytical Data Science fresher with a strong foundation in Python, SQL, Statistics, Pandas, NumPy, and Data Visualization, passionate about solving real-world business problems using data.

- 🔗 [LinkedIn](https://www.linkedin.com/in/krishna-babu-elarapu-619457355/)
- 💻 [GitHub](https://github.com/krishnababuelarapu-bit)

---

⭐ If you found this project useful, consider giving it a star!
