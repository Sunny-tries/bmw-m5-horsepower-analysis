# BMW M5 Web-Scraping and Data Visualization Project

## Overview
This project demonstrates how to collect, clean, and visualize real-world data using **web scraping, Python data manipulation, and Excel visualization** techniques. It was created as my first post on my Instagram page, **GraficalStories**, to showcase my journey in mastering data analysis and visualization.

The goal is to strengthen my skills in **data scraping and Excel visualization** while continuing my job search for a data analyst position. The dataset focuses on the **horsepower evolution of the BMW M5** across various generations, providing insights into how BMW's iconic performance sedan has evolved.

---

## Table of Contents
1. [Project Goal](#project-goal)  
2. [Tech Stack](#tech-stack)  
3. [Data Collection](#data-collection)  
4. [Data Cleaning and Preparation](#data-cleaning-and-preparation)  
5. [Missing Data Handling](#missing-data-handling)  
6. [Visualizations](#visualizations)  
7. [How to Run the Project](#how-to-run-the-project)  
8. [Future Improvements](#future-improvements)  

---

## Project Goal
This project aims to explore the **horsepower trends** of BMW M5 models across generations by:
1. **Scraping data** from the [Horsepower Specs website](https://www.horsepowerspecs.com/model/bmw-m5/).
2. **Cleaning and transforming the data** to prepare it for analysis.
3. **Handling missing data** by researching and adding it manually.
4. **Creating visualizations** using **Excel** to communicate insights.

---

## Tech Stack
- **Python**: Web scraping, data cleaning, and export to Excel.  
  - Libraries: `pandas`, `BeautifulSoup`, `requests`, `os`
- **Excel**: Used for data visualization (line chart and bar chart).

---

## Data Collection
The data was scraped from [Horsepower Specs](https://www.horsepowerspecs.com/model/bmw-m5/) using **Python’s BeautifulSoup** library. Specifically:
- **Horsepower** values and **RPM** readings were extracted from HTML elements.
- **Model years** and **generation codes** (e.g., E34, F90) were scraped to align the data with the correct car generations.

---

## Data Cleaning and Preparation
The web scraping returned a lot of raw HTML that needed to be processed. Below are the key cleaning steps:
1. **Strip HTML tags** to extract horsepower values.
2. **Extract years and model names** to ensure proper matching of data.
3. **Transform data into a DataFrame** using `pandas` to make it suitable for further processing.

--- 
## Missing Data Handling
During the data scraping process, I discovered that the earliest BMW M5 generations (E12 and E28) were not available on the website. To fill in the missing data:

- I researched these models independently.
- Manually added their horsepower values to the DataFrame.

---

## Visualizations
The cleaned data was exported to Excel, where two visualizations were created:

- Line Chart: Showcasing the horsepower growth across different generations (from E12 to F90).
- Bar Chart: Highlighting the change in horsepower from one generation to the next. The biggest increase was observed in the E60 model, which saw a jump of 106 hp compared to the E39.

---
## Future Improvements
- Automate data updates: Schedule periodic scrapes to update the dataset with any new models or changes.
- Additional metrics: Include more performance data (e.g., 0-60 mph times or torque figures) for deeper insights.
- Interactive Dashboards: Explore Power BI or Tableau for richer, interactive visualizations.
- Expand to other BMW models: Include other M models like the M3 or M8 to compare across the entire M lineup.
