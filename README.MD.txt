# Netflix Content Growth Dashboard (Power BI)

![Dashboard](images/dashboard.png)

## Overview
An interactive Power BI dashboard analyzing Netflix's catalog of 8,791 titles. It shows how content has grown by release year and how the catalog splits between Movies and TV Shows.

## Business Questions
- How has the number of titles changed by release year?
- What is the split between Movies and TV Shows?
- How fast is the catalog growing year over year (YoY) and cumulatively?

## Dashboard Sections
1. **Titles by release year**: trend of titles released each year
2. **Movies vs TV Shows**: catalog composition by content type
3. **Growth insights**: YoY change and cumulative titles (DAX measures)

## Dataset
- Netflix Titles dataset (Kaggle): add the link here
- 8,791 rows and 10 columns after cleaning: `show_id, type, title, director, country, date_added, release_year, rating, duration, listed_in`
- Titles added to Netflix between Jan 2008 and Sep 2021

## Data Cleaning
- Replaced missing `director` and `country` values with "Unknown"
- Converted `date_added` to a date type
- Standardized data types and removed duplicates (`show_id` is unique)
- Saved the result as `Cleaned_Dataset.xlsx` and loaded it into Power BI

## Key Insights
- Movies make up about **70%** of the catalog (6,126 titles) and TV Shows about **30%** (2,664).
- Release volume peaked in **2018 with 1,146 titles**, followed by 2017 and 2019 (1,030 each).
- About **71%** of all titles were released in 2015 or later, so the catalog is heavily recent.
- The **United States (3,239)** and **India (1,057)** are the top content-producing countries.
- **TV-MA** is the most common rating (3,205 titles).

## DAX Measures
- `YoY Change`: year-over-year change in the number of titles
- `Cumulative Titles`: running total of titles by release year

## Tools
Power BI Desktop · DAX · Excel (data cleaning)

## Repository Structure
```
├── dashboard/Netflix_Dashboard.pbix
├── data/Cleaned_Dataset.xlsx
├── images/dashboard.png
└── README.md
```

## How to Use
Download the `.pbix` file and open it in Power BI Desktop (free).

## Author
HanyOver