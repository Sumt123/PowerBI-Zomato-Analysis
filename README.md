# Zomato Power BI Analysis Project

This project showcases a comprehensive Power BI dashboard built using data from Zomato. It includes advanced data cleaning, transformation, DAX measures, and interactive visualizations to provide business insights across global restaurants.

---

## Project Objective

To create a consolidated, clean, and interactive Power BI dashboard that allows stakeholders to assess global restaurant data across various metrics such as cost, rating, cuisine type, and geographical spread.

---

## Tools Used

- Power BI Desktop  
- Power Query (M Language)  
- DAX (Data Analysis Expressions)  
- Excel (Source Files)

---

## Dataset Source

All raw datasets were obtained from the following repository:  
**[Power BI Datasets – Simplilearn GitHub Repo](https://github.com/Simplilearn-Edu/Power-BI-Datasets.git)**

---

## Data Overview

Originally, 8 tables were provided. These were transformed and cleaned to form 4 major tables:

1. **Continent Table** – Contains restaurant details with geographic and cuisine data.  
2. **KPIs Table** – Includes cost, ratings, delivery details, and user votes.  
3. **Country Master Table** – Maps countries to continent and country code.  
4. **Cuisine Table** – Extracted from original continent data, shows cuisines per restaurant.

---

## Data Cleaning & Transformation

- Corrected city name errors:
  - `Sí£o Paulo` → `São Paulo`
  - `ÛÁstanbul` → `Istanbul`
  - `Cedar Rapids/Iowa City` → `Cedar Rapids`
- Split `Restaurant Name and Address` from a combined column.
- Removed duplicate and null values.
- Removed unused columns.
- Created unique lists for dimension tables (Country Master, Cuisine Table).
- Normalized cuisine data by splitting and unpivoting cuisine columns.
- Created separate `Cuisine Table` using Restaurant ID and Cuisine values only.

---

## Data Modeling

- Built relationships between fact and dimension tables using keys such as `Restaurant ID` and `Country Code`.
- Followed a star schema model for performance and clarity.
- Ensured proper data types and lookup table configuration.

---

## DAX Measures & Columns

### New Columns

- `Rating Color` (Based on Aggregate Rating):
  - > 4.5 → Dark Green
  - 4.0 to 4.4 → Green  
  - Below 4.0 → Others
- `Continent` column in Country Master (Created manually)
- `Cuisine Count` in Cuisine Table
- `Restaurant Count` in Continent Table

### DAX Measures

- `Restaurant Count`
- `Average Cost`
- `Average Rating`
- `Cuisine Count`

---

## Dashboard Pages

### Page 1 – Zomato Overview Dashboard

**KPI Cards:**
- Total Restaurants: 9551
- Cuisine Count: 249
- Average Rating: 2.67
- Average Cost: ₹1.20K

**Visualizations:**
- World Map – Global Restaurant Distribution by Country
- Tree Map – Distribution of Restaurants by Cuisine (Top: North Indian, Chinese, Café)
- Table – Top Restaurants by Rating (e.g., Zolocrust, Yellow Dog Eats, Urbanology)
- Table – Lower Rated Restaurants (e.g., Amul Ice Cream Parlour, Agrawal Bikaner Sweets)

**Slicers:**
- Continent
- Country
- City
- Cuisine

---

### Page 2 – Zomato Business Insight Dashboard

**KPI Cards:**
- Total Continents: 6
- Total Countries: 15
- Total Cities: 140
- Total Votes: ~1 Million

**Visualizations:**
- Table – Restaurants with High Average Cost for two person (e.g., Satoo, Shangri-La, Sushi Masa)
- Table – Lowest Cost Restaurants for two person (e.g., Texas RT Chowk)
- Pie Chart – Online Delivery Availability (Yes: 25%, No: 75%)
- Clustered Column & Line Chart – Cuisine Served Count & Restaurant Rating
  - Top Cuisine Providers: Subway, Domino's Pizza, Haldiram, Green Chick Chop
- Clustered Bar Chart - Restauran Count by Rating Color

---

## Key Insights

- 75% of restaurants do **not offer** online delivery.
- Top 3 cuisines globally: **North Indian**, **Chinese**, **Café**.
- Some restaurants charge above ₹4 lakh for two people.
- High-rated restaurants include **Zolocrust**, **Urbanology**, and **Yellow Dog Eats**.
- **Dominos** and **Subway** offer a wide variety of cuisines.
- Very less number of restaurants are top rated 1000 approx out of 9000.

## Final conclusion:

-The Power BI project successfully transformed raw Zomato data into a clean, interactive dashboard that offers key insights global restaurant trends. By applying data cleaning , transformation, DAX measures , and effective visualization, the report enables stakeholders to understand restaurant performance , customer ratings, cuisine preferance , and business potential across different countries and continents.

## Author

**Sumit Kumar Yadav**  
Email: [sumitky9305@gmail.com](mailto:sumitky9305@gmail.com)  
Linkdin: [www.linkedin.com/in/sumit-yadav-888a14284]
GitHub: [Sumit123]

---

## Screenshots

*
![WhatsApp Image 2025-04-24 at 2 12 16 AM](https://github.com/user-attachments/assets/97c07879-29bc-4216-a677-c52bfc3ca9fd)

---
![WhatsApp Image 2025-04-24 at 2 12 17 AM](https://github.com/user-attachments/assets/67daf37f-d5b8-4995-81e9-2052b831bd62)

## License

This project is for educational and demonstration purposes only.

