📊 OTT Content Analytics Dashboard

An end-to-end Data Analytics project analyzing OTT platform content using SQL (SQLite), Excel, and Power BI.
The project focuses on understanding content performance, genre popularity, country-wise distribution, and year-wise trends through interactive dashboards.

🎯 Project Objective

The objective of this project is to analyze OTT content data and answer key business questions:

Which genres are most popular on OTT platforms?

Which countries contribute the most content?

How do ratings and content duration vary across genres and countries?

What trends exist in OTT content releases over the years?

🛠️ Tools & Technologies Used

SQL (SQLite) – Data storage, querying & aggregation

Microsoft Excel – Exploratory Data Analysis (EDA) & Excel dashboard

Power BI – Interactive dashboards & visual analytics

GitHub – Version control & project hosting

📂 Project Structure
ott-content-analytics-dashboard/
│
├── Dashboard/
│   ├── dashboard_images/
│   │   ├── OTT Content Analytics Dashboard.jpg
│   │   ├── Genre Analysis Dashboard.jpg
│   │   ├── Country Analysis Dashboard.jpg
│   │   └── Year-wise Trend Dashboard.jpg
│   │
│   └── OTT_Content_Analysis_Dashboard.pbix
│
├── Data/
│   ├── ott_analysis_clean.db
│   ├── ott_analysis_clean.sqbpro
│   └── ott_content_dataset.csv
│
├── Excel/
│   └── OTT_Content_Performance_Analysis.xlsx
│
├── SQL/
│   └── SQL_Queries.sql
│
└── README.md

📊 Power BI Dashboards
🔹 1. OTT Content Overview Dashboard

Provides a high-level summary of OTT content performance.

Metrics Included:

Total Titles

Average Rating

Highest Rating

Average Duration

Overall content insights

🔹 2. Genre Analysis Dashboard

Analyzes content performance across different genres.

Insights:

Total titles by genre

Average rating by genre

Average duration by genre

Top-rated genres

🔹 3. Country Analysis Dashboard

Shows country-wise content distribution and performance.

Insights:

Total titles by country

Average rating by country

Average duration by country

Country-wise content contribution

🔹 4. Year-wise Trend Dashboard

Displays OTT content trends over time.

Insights:

Titles released per year

Rating trends over time

Duration trends over time

📈 Excel Dashboard (EDA)

An Excel-based dashboard was created for initial data exploration and validation before Power BI development.

Includes:

Summary KPIs

Genre & country analysis

Year-wise trends

Interactive slicers

🧮 SQL Analysis

SQL queries were used to aggregate and analyze OTT content data.

Example Query:

SELECT genre, COUNT(*) AS total_titles
FROM ott_content
GROUP BY genre
ORDER BY total_titles DESC;

🔍 Key Insights

Crime and Drama genres dominate OTT platforms

USA and UK contribute the highest number of titles

Ratings remain relatively consistent across genres

Average content duration shows a gradual increase over time

🎓 Learning Outcomes

Hands-on experience with SQL analytics

Practical Excel dashboard development

Building multi-page Power BI dashboards

Understanding a real-world data analytics workflow

Creating a portfolio-ready GitHub project

👤 Author

Ashok Suravarapu
BCA – Data Analytics

## 🧮 SQL Queries Used

```sql
-- Total Titles
SELECT COUNT(*) AS total_titles FROM ott_content;

-- Average Rating
SELECT ROUND(AVG(rating), 2) AS avg_rating FROM ott_content;

-- Highest Rating
SELECT MAX(rating) AS highest_rating FROM ott_content;

-- Titles by Genre
SELECT genre, COUNT(*) AS total_titles
FROM ott_content
GROUP BY genre
ORDER BY total_titles DESC;

-- Titles by Country
SELECT country, COUNT(*) AS total_titles
FROM ott_content
GROUP BY country
ORDER BY total_titles DESC;

-- Year-wise Trend
SELECT release_year, COUNT(*) AS total_titles
FROM ott_content
GROUP BY release_year
ORDER BY release_year;
---


