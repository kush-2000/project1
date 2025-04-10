# 🌍 COVID-19 Data Analysis (Dec 2019 – Nov 2020)

This project explores the global impact of COVID-19 using two datasets:  
- **New Daily Cases**  
- **New Daily Deaths**

Each dataset contains daily COVID-19 statistics for nearly every country in the world, spanning from **December 31, 2019 to November 29, 2020**. Columns represent individual countries, while rows track the evolving case and death counts by date.

---

## 📊 Why This Dataset?

I chose to analyze COVID-19 data because the pandemic has been a transformative global event, impacting every aspect of our lives. While I've seen numerous charts and dashboards during the last few years, this is my first time conducting my own in-depth analysis of the raw data. With global coverage, this dataset allows for meaningful comparisons between countries and across time.

---

## 🛠️ Key Steps & Tools Used

- **Data Wrangling & Tidying**
  - Merged `new_cases` and `new_deaths` datasets using `full_join()`
  - Converted data from wide to long format using `pivot_longer()` and then retidied using `pivot_wider()`
  - Cleaned column names and added a new `ratio` column for deaths/cases

- **Exploratory Data Analysis**
  - Identified top countries by total cases and deaths
  - Summarized mean, median, standard deviation, max, and min of daily cases/deaths
  - Filtered for specific countries like China and the US
  - Used `stringr` functions to manipulate country names

- **Visualizations**
  - Bar charts for top countries with most cases
  - Scatter plots to explore death vs. case relationships
  - Monthly case comparison plots between US and Italy
  - Demonstrated how y-axis scaling can influence interpretation

---

## 📈 Insights

- The **United States** had the highest total number of cases and deaths.
- **France** showed high case counts but lower deaths — potentially indicating stronger healthcare systems or reporting methods.
- Two major waves were observed:
  - **First Wave:** Around July 2020
  - **Second Wave:** October–November 2020
- Monthly trends helped visualize when each country was hit the hardest and how quickly it rebounded.

---

## ⚠️ Limitations

- Reporting standards varied by country.
- Some countries may have underreported cases and deaths.
- Data only covers **Dec 31, 2019 – Nov 29, 2020** — missing later waves and vaccination effects.

---

## 📌 Conclusion

This project demonstrates how data wrangling, summarization, and visualization can uncover powerful insights about global trends. With just two CSV files, we can analyze pandemic progression across 214 countries, visualize waves, and compare responses. This was not only a great exercise in working with messy real-world data in **R**, but also a way to understand the broader global narrative of COVID-19 from a data perspective.

---

> Built using **R**, **tidyverse**, and a passion for learning through data.
