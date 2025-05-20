# Zomato Power BI Analysis Project

    This project demonstrates a comprehensive Power BI dashboard designed to extract actionable insights from global Zomato restaurant data. By leveraging advanced data cleaning, transformation (Power Query), DAX measures, and interactive visualizations, the dashboard provides a strategic overview for stakeholders to optimize business decisions.
---

## Project Objective

    To develop a consolidated, clean, and interactive Power BI dashboard that enables stakeholders to quickly assess global restaurant performance, customer preferences, and market potential across various metrics such as cost, rating, cuisine type, and geographical distribution. The ultimate goal is to empower data-driven strategies for restaurant growth and customer satisfaction.

---

## Tools & Technologies

- **Data Source:** Excel (Raw Zomato Datasets)
- **Data Preparation & Transformation:** Power Query (M Language)
- **Data Modeling & Analysis:** DAX (Data Analysis Expressions)
- **Visualization & Reporting:** Power BI Desktop
---

## Dataset Source

All raw datasets were obtained from the following repository:  
**[Power BI Datasets – Simplilearn GitHub Repo](https://github.com/Simplilearn-Edu/Power-BI-Datasets.git)**

---

## Dataset Overview

Initially comprising 8 raw tables, the data was meticulously transformed and consolidated into 4 key analytical tables:

1. **Continent Table** – Contains restaurant details with geographic and cuisine data.  
2. **KPIs Table** – Contains key performance indicators such as cost for two, ratings, delivery availability, and user votes.  
3. **Country Master Table** – Maps countries to continents and country codes for regional analysis.
4. **Cuisine Table** – A normalized dimension table showing cuisine types associated with each restaurant.

---

## Data Cleaning & Transformation

  ## Rigorous data cleaning and transformation were crucial to ensure data integrity and usability:

 **Standardized City Names:** Corrected inconsistencies like "Sí£o Paulo" to "São Paulo" and "ÛÁstanbul" to "Istanbul."
 **Data Structuring:** Split combined "Restaurant Name and Address" columns for granular analysis.
 **Quality Assurance:** Eliminated duplicate and null values; removed irrelevant columns to streamline the dataset.
 **Dimensional Modeling:** Created unique lists for dimension tables (Country Master, Cuisine Table) to support a robust star schema.
 **Cuisine Normalization:** Efficiently processed and unpivoted cuisine data, creating a clean, separate "Cuisine Table" to support flexible analysis.

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
- **Total Restaurants:** 9551
- **Cuisine Count:** 249
- **Average Rating:** 2.67
- **Average Cost:** ₹1.20K

**Visualizations:**
- **World Map** – Global Restaurant Distribution by Country
- **Tree Map** – Distribution of Restaurants by Cuisine (Top: North Indian, Chinese, Café)
- **Table** – Top Restaurants by Rating (e.g., Zolocrust, Yellow Dog Eats, Urbanology)
- **Table** – Lower Rated Restaurants (e.g., Amul Ice Cream Parlour, Agrawal Bikaner Sweets)

**Slicers:**
- Continent
- Country
- City
- Cuisine

---

### Page 2 – Zomato Business Insight Dashboard

**KPI Cards:**
- **Total Continents:** 6
- **Total Countries:** 15
- **Total Cities:** 140
- **Total Votes:** ~1 Million

**Visualizations:**
- **Table** – Restaurants with High Average Cost for two person (e.g., Satoo, Shangri-La, Sushi Masa)
- **Table** – Lowest Cost Restaurants for two person (e.g., Texas RT Chowk)
- **Pie Chart** – Online Delivery Availability (Yes: 25%, No: 75%)
- **Clustered Column & Line Chart** – Cuisine Served Count & Restaurant Rating
- **Top Cuisine Providers** - Subway, Domino's Pizza, Haldiram, Green Chick Chop
- **Clustered Bar Chart** - Restauran Count by Rating Color

---

## Key Business Insights & Recommendations

## This analysis uncovered several critical insights with direct business implications:

**Untapped Online Delivery Market:** A striking **75%** of restaurants do not offer online delivery, presenting a massive opportunity for delivery platforms or restaurants looking to expand services. 
**Recommendation:** Focus marketing and partnership efforts on expanding online delivery options in underserved regions.
**Dominant Cuisine Preferences:** North Indian, Chinese, and Café are the top three globally consumed cuisines. 
**Recommendation:** Restaurants specializing in these cuisines have higher market appeal; new ventures could prioritize these.
**Cost Variance & Market Segmentation:** Significant cost disparities exist, with some restaurants charging substantially higher(**e.g.** 4 lakh for two people).
**Recommendation:** Target specific consumer segments based on price point, or analyze pricing strategies for competitiveness.
**High-Rated Restaurant Benchmarks:** Identifying top-rated establishments like Zolocrust and Urbanology provides benchmarks for service quality and customer satisfaction. **Recommendation:** Study characteristics of high-rated restaurants to replicate success factors.
**Brand Reach vs. Rating:** While brands like Domino's and Subway offer a wide variety of cuisines, their overall average ratings might vary.
**Recommendation:** Monitor customer feedback closely for chain restaurants to ensure consistent quality across locations.
**Rating Distribution Challenge:** Only a small percentage of restaurants (approx. 1,000 out of 9,000+) are highly rated.
**Recommendation:** Implement quality improvement initiatives for lower-rated establishments and promote best practices from top performers.

## Final conclusion:

    This Power BI project successfully transformed raw Zomato data into a clean, interactive, and insight-rich dashboard. By applying robust data cleaning, transformation, DAX measures, and effective visualization techniques, the report empowers stakeholders with a deep understanding of global restaurant performance, customer ratings, cuisine preferences, and market potential. The identified insights can directly inform strategic decisions related to service expansion, marketing efforts, and operational improvements, ultimately driving business growth in the competitive food industry.

## Author

**Sumit Kumar Yadav**  
**Email:** [sumitky9305@gmail.com](mailto:sumitky9305@gmail.com)  
**Linkdin:** [www.linkedin.com/in/sumit-yadav-888a14284]
**GitHub:** [Sumit123]

---

## Screenshots

*
![WhatsApp Image 2025-04-24 at 2 12 16 AM](https://github.com/user-attachments/assets/97c07879-29bc-4216-a677-c52bfc3ca9fd)

---
![WhatsApp Image 2025-04-24 at 2 12 17 AM](https://github.com/user-attachments/assets/67daf37f-d5b8-4995-81e9-2052b831bd62)

## License

This project is for educational and demonstration purposes only.

