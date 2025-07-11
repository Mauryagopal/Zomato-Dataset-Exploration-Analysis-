# 🍽️ Zomato Dataset Analysis using SQL Server

This project focuses on exploratory data analysis (EDA) and deriving insights from the Zomato dataset using **SQL Server**. Zomato is a leading Indian multinational food delivery and restaurant aggregator platform. The dataset contains information about over 9000 restaurants across multiple countries. The objective is to understand restaurant distribution, customer preferences, services offered, and pricing trends.

---

## 📊 Dataset Overview

The dataset contains more than **9000 rows** and includes the following columns:

- `RestaurantID`
- `RestaurantName`
- `City`
- `Location`
- `Cuisines`
- `CountryCode`
- `Rating`, `Votes`, `Currency`
- and more...

---

## 🛠️ SQL Data Exploration

Key steps performed during the data exploration phase:

- ✅ Checked table structure: column names, data types, constraints
- 🔁 Identified and removed duplicate values in `RestaurantID`
- 🧹 Removed irrelevant/unwanted columns
- 🔗 Merged two tables using `CountryCode` to add the `CountryName` column
- ✏️ Corrected misspelled city names
- 📈 Used **window functions** to create rolling counts of restaurants
- 📊 Calculated min, max, and average values for `Votes`, `Rating`, and `Currency`
- 🏷️ Created a new column to classify restaurants based on ratings

---

## 🔍 Key Insights

- 🇮🇳 **India accounts for 90.67%** of the restaurant data, followed by the USA (4.45%)
- 🌍 Out of 15 countries, only 2 support **online delivery**:
  - India: 28.01% restaurants
  - UAE: 46.67% restaurants
- 📍 **Top Indian locations** by restaurant count:
  - Connaught Place, New Delhi – 122 restaurants
  - Rajouri Garden – 99
  - Shahdara – 87
- 🍛 **Most popular cuisine** in Connaught Place: North Indian
- 🪑 **Table Booking (Connaught Place)**:
  - 54 out of 122 restaurants provide table booking
  - Avg. rating with table booking: **3.9**
  - Avg. rating without table booking: **3.7**
- 🥇 **Best moderately-priced Indian restaurant**:
  - **India Restaurant**, Kolkata, India
  - `RestaurantID`: 20747
  - Avg. cost for two: **< ₹1000**
  - Rating: **> 4**
  - Votes: **> 4**
  - Offers both **table booking** and **online delivery**

---

## 🧑‍💻 Tools Used

- SQL Server  
- Microsoft Excel

---

## 📁 Project Structure
Zomato_SQL_Analysis/
│
├── SQL_Queries/
│ ├── Data_Exploration.sql
│ ├── Data_Cleaning.sql
│ ├── Insights_Generation.sql
│
├── Dataset/
│ └── Zomato_Dataset.csv

## 📌 Future Enhancements

- Add Power BI or Tableau dashboards for better visualization
- Build a cuisine-based recommendation engine
- Extend analysis with pricing trends across cities and countries

## 📬 Contact

**Gopal Maurya**  
B.Tech Biomedical Engineering, NIT Rourkela
