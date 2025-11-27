# Naukri.com Analysis

## Task Overview
This project focuses on **scraping Data Analyst job listings** from a real job portal using Python and BeautifulSoup. The scraped data is cleaned, analyzed, and visualized to provide insights into top locations, in-demand skills, and hiring trends.

## Objective
- Scrape job listings for Data Analyst roles including:
  - Job Title
  - Company Name
  - Location
  - Salary (if available)
  - Required Skills
- Clean and preprocess the collected data.
- Perform basic analysis and visualize key insights.


## Tools & Libraries
- **Python**
- **Libraries:**
  - `requests` – To fetch web pages
  - `BeautifulSoup` – To parse HTML
  - `pandas` – For data cleaning and analysis
  - `matplotlib` – For data visualization
  - `collections.Counter` – To count skill frequency
  - `re` – For text cleaning using regex
  - `time` – To avoid overloading the server


## Data Collection & Cleaning
- Used `requests` to fetch HTML content and `BeautifulSoup` to parse it.
- Extracted job title, company, location, salary, and skills.
- Cleaned text using `.text.strip()` and regex (`re`) for skill extraction.
- Used `time.sleep(1-2)` seconds between requests to avoid being blocked.
- Removed duplicates and null values.
- Converted cleaned data into a pandas DataFrame for analysis.

## Data Analysis & Visuals
- Counted job listings by location to find top 5 hiring cities.
- Extracted and counted skill frequency using `Counter`.
- Visualized results:
  - **Bar Chart / Pie Chart:** Top 5 job locations
  - **Bar Chart:** Most in-demand skills


## Key Findings
- **Total Jobs Scraped:** [e.g., 500]
- **Top Locations:** [Example: New York, San Francisco, Remote, Chicago, Austin]
- **Most In-Demand Skills:** Python, SQL, Excel, Power BI, Tableau


## Challenges Faced
- Dynamic web pages may require extra parsing logic.
- Rate-limiting by the website – handled using `time.sleep()`.
- Inconsistent skill formatting across job listings – required text cleaning with regex.
- Handling missing salary and location data.


## Future Work
- Expand scraping to multiple job portals to increase dataset size.
- Use NLP techniques to analyze skill requirements more deeply.
- Build interactive dashboards for dynamic visualization of insights.


