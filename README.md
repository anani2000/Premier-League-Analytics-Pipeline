# Premier-League-Analytics-Pipeline(5 Seasons)

This project provides an end-to-end data pipeline for extracting, processing, and visualizing English Premier League data from the last five seasons. It automates web scraping, cleaning, merging, and analytics to create a Power BI dashboard for team and player performance comparisons.

## Key Features

### Data Pipeline

* Source: Data scraped from FBref.com (dynamically loaded HTML tables).
* Scraping Method:

  * Used CloudScraper to bypass Cloudflare protection.
  * Parsed hidden HTML tables with multi-index structures.
* Data Processing (Python):

  * Cleaned, normalized, and merged datasets across 5 Premier League seasons (2019/20 – 2023/24).
  * Exported a consolidated CSV file ready for Power BI.

## Project Structure

```
PremierLeague-Data-Pipeline-Python-to-PowerBI/
├── data/
│   └── premier_league_5_seasons.csv
├── notebooks/
│   └── PFL_Data_Extraction and Cleaning.ipynb
│   └── PFL_Data_Extraction and Cleaning.py
├── powerbi/
│   └── PFL_Analysis.pbix
│   └─ Images
├── README.md
└── requirements.txt
```

## Power BI Dashboard Overview

The dashboard contains 5 interactive pages:

| Page Name                       | Description                                                                                                  |
| ------------------------------- | ------------------------------------------------------------------------------------------------------------ |
| Home Page                       | Overview of league stats for all seasons (total goals, matches, best players, etc.)                          |
| Players Comparison         | Compare any two or more players based on goals, assists, minutes, xG, xA, etc.                               |
| Teams statistics | Team-level stats derived from player performance (most goals from players, most red cards, assists per team) |
| Player In-Depth Analysis        | Individual player's trend line over 5 seasons (progress in goals, assists, xG, form)                         |
| Player Statistics           | Leaderboards and Insights for top goals, assists, progressive passes, key passes, etc.                                    |

## Technologies Used

| Process                   | Tools & Libraries                             |
| ------------------------- | --------------------------------------------- |
| Web Scraping              | Python, CloudScraper, Requests|
| Data Processing           | Pandas, NumPy, matplotlib.pyplot, seaborn                                 |
| Visualization & Reporting | Power BI                                      |
| Export Format             | CSV, Power BI (.pbix)                         |
| League Data               | FBref.com                    |

## Setup / Installation

To run the data pipeline and reproduce the dataset, install the required Python libraries:

```
pip install cloudscraper==1.2.71
pip install requests==2.32.4
pip install pandas==2.2.2
pip install numpy==2.0.2
pip install time
```

Or, if you have a requirements.txt file, run:

```
pip install -r requirements.txt
```

## How to Run the Pipeline

1. Clone the repository

   ```
   ```

git clone [https://github.com/](https://github.com/)<your-username>/Premier-League-Analytics-Pipeline.git


```

2. Run the scraping and cleaning notebook/script
```

python PFL_Data_Extraction and Cleaning.py

```

3. Open Power BI file
```

/powerbi/PFL_Analysis.pbix

```

4. Update data source in Power BI if the file path changes.
```
## Future Enhancements

- Automate pipeline with Airflow or Prefect
- Add live data updates from ongoing seasons
- Deploy dashboard online using Power BI Service or Streamlit
- Add predictive analysis (player performance forecasts, win probability)
- Add data for Goalies

## Contact

Author: Karim Anani  
Email: KarimAnani2024@gmail.com  
 GitHub: https://github.com/anani2000

```
