# Olympic Insights Using Data Analytics

![Power BI](https://img.shields.io/badge/Power%20BI-Data%20Visualization-F2C811?logo=powerbi&logoColor=black)
![Dashboard](https://img.shields.io/badge/Dashboard-6%20Pages-blue)
![Status](https://img.shields.io/badge/Status-Completed-success)

## Project Overview

Olympic Insights Using Data Analytics is an interactive six-page Power BI project developed to analyze historical Olympic performance.

The dashboard provides insights into athlete participation, country-wise medal performance, leading athletes, sport-specific dominance, host-country performance, and gender and age demographics.

## Problem Statement

The International Olympic Committee requires an analytical solution to evaluate athlete performance, country-wise medal trends, sport-specific dominance, host-country outcomes, and demographic participation patterns across different Olympic Games.

The objective of this project is to transform historical Olympic data into an interactive and easy-to-understand Power BI dashboard for performance monitoring and strategic analysis.

## Project Objectives

- Track Olympic editions, events, countries, athletes, and medals.
- Compare country-wise medal performance and medal efficiency.
- Identify top-performing and most-participated athletes.
- Analyze sport-wise medal and athlete participation trends.
- Evaluate country dominance across different sports.
- Compare host and non-host medal performance.
- Analyze male and female participation over time.
- Explore medal winners across different athlete age groups.

## Dashboard Preview

### 1. Global Medal Overview

This page provides a high-level overview of Olympic editions, total events, participating countries, leading medal-winning countries, and historical medal trends.

![Global Medal Overview](<img width="1325" height="741" alt="01-global-medal-overview" src="https://github.com/user-attachments/assets/7b966034-0c2d-4b13-b374-0beada19954b" />
)

### 2. Country Insights

This page analyzes country-level athlete representation, medal efficiency, medal distribution, leading sports, and year-wise medal performance.

![Country Insights](<img width="1322" height="742" alt="02-country-insights" src="https://github.com/user-attachments/assets/86d2e54e-a3f4-4fde-945a-ba827dde5884" />
)

### 3. Athlete Spotlight

This page highlights leading medal-winning athletes, Olympic appearances, medal-winning age groups, gender distribution, and the youngest and oldest medal winners.

![Athlete Spotlight](<img width="1325" height="742" alt="03-athlete-spotlight" src="https://github.com/user-attachments/assets/16cdd401-1cd0-4ac4-aead-b923a5f2103c" />
)

### 4. Sport & Event Analysis

This page explores sport-wise medal trends, athlete participation, top sports, and country dominance across different Olympic sports.

![Sport and Event Analysis](<img width="1325" height="742" alt="04-sport-event-analysis" src="https://github.com/user-attachments/assets/9c5296d9-150c-4b02-a302-20218cef26fe" />
)

### 5. Host Country Analysis

This page examines Olympic hosting patterns and compares the medal performance of host and non-host countries.

![Host Country Analysis](<img width="1330" height="742" alt="05-host-country-analysis" src="https://github.com/user-attachments/assets/39be4816-2763-4e2f-9d75-ffcd0e151059" />
)

### 6. Gender & Demographics

This page analyzes male and female athlete participation, gender-wise medal winners, leading sports by gender, and athlete participation across age groups.

![Gender and Demographics](<img width="1323" height="742" alt="06-gender-demographics" src="https://github.com/user-attachments/assets/3806491b-1a7f-4630-b3fd-06faa931d9a9" />
)

## Dataset Information

The project was developed using six Olympic CSV datasets:

| Dataset | Description |
| --- | --- |
| `Olympic_Athlete_Bio.csv` | Athlete profile and demographic information |
| `Olympic_Athlete_Event_Results.csv` | Athlete-level participation and medal results |
| `Olympic_Games_Medal_Tally.csv` | Official country medal tally by Olympic edition |
| `Olympic_Results.csv` | Olympic event and result information |
| `Olympics_Country.csv` | Country and NOC reference information |
| `Olympics_Games.csv` | Olympic edition, year, city, season, and host information |

The raw CSV files are not stored in this repository because some source files exceed GitHub's browser upload limit.

### Dataset Download

The complete dataset can be downloaded from the following source:

[Download Olympic Games Dataset](https://wscubetechpvtltd-my.sharepoint.com/:u:/g/personal/ayushi_jain_wscubetech_com/IQB5a0BuQu_2Vl4AL0dx6jKzAcgH6eQOsf8J2JsVvpby0sY?e=pcLSiD)

> The dataset is used for educational and portfolio purposes. Dataset ownership remains with its respective source.

## Dataset Size and Coverage

The supplied datasets contain approximately:

- 156K athlete biography records
- 316K athlete-event participation records
- 44.7K athlete-level medal records
- 112 sports
- 231 participating NOC codes
- 64 Olympic editions in the Games table

## Important Medal Definition

This project contains two different medal-counting levels:

1. **Athlete-Level Medals:** Each medal-winning athlete is counted individually. Members of a medal-winning team can therefore contribute multiple athlete-level medal records.

2. **Official Country Medals:** A team medal is counted once in the official country medal tally.

Therefore, athlete-level medal totals and official country medal totals should not be interpreted as identical metrics.

## Data Preparation

The data was cleaned and transformed using Power Query.

The preparation process included:

- Correcting source paths.
- Assigning appropriate data types.
- Checking missing and inconsistent values.
- Removing unnecessary columns.
- Standardizing country, sport, medal, and gender fields.
- Creating supporting year and age-group fields.
- Preparing host and non-host classifications.
- Building relationships across multiple Olympic tables.

## Data Model

The Power BI data model connects the datasets using common identifiers such as:

- `athlete_id`
- `edition_id`
- `result_id`
- `country_noc`
- `noc`

These relationships support cross-table filtering and interactive analysis across athletes, countries, sports, events, Olympic editions, and medal records.

## DAX and Analytical Calculations

DAX measures and calculated fields were used for:

- Total athletes
- Total medals
- Total countries
- Total events
- Gold, silver, and bronze medals
- Medal efficiency
- Medal-winning athletes
- Olympic appearances
- Running total of medals
- Average athlete age
- Sport-wise participation
- Host and non-host medal comparison
- Gender-wise participation and medal analysis

## Dashboard Features

- Six analytical report pages
- Page navigation buttons
- Interactive year, season, country, sport, athlete, and gender slicers
- KPI cards
- Top-N rankings
- Historical trend analysis
- Running-total analysis
- Cross-filtering between visuals
- Country and sport-level comparisons
- Athlete age and gender analysis
- Consistent dashboard theme and layout

## Tools and Technologies

- **Microsoft Power BI Desktop** – Dashboard development
- **Power Query** – Data cleaning and transformation
- **DAX** – Measures, KPIs, rankings, and calculations
- **Data Modeling** – Table relationships and filter flow
- **CSV** – Raw data sources
- **GitHub** – Project documentation and portfolio hosting

## Repository Structure

```text
olympic-insights-power-bi/
├── README.md
├── dashboard/
│   └── olympic.pbix
├── screenshots/
│   ├── 01-global-medal-overview.png
│   ├── 02-country-insights.png
│   ├── 03-athlete-spotlight.png
│   ├── 04-sport-event-analysis.png
│   ├── 05-host-country-analysis.png
│   └── 06-gender-demographics.png
├── docs/
│   └── Olympic_Insights_Dashboard.pdf
└── data/
    └── README.md
```

## How to View the Project

### View without Power BI

Dashboard pages can be viewed directly through the screenshots folder or the PDF report:

- Open the `screenshots` folder to view individual dashboard pages.
- Open `docs/Olympic_Insights_Dashboard.pdf` to view the complete report.

### Open the Interactive Power BI Dashboard

1. Download this repository.
2. Install Microsoft Power BI Desktop.
3. Open `dashboard/olympic.pbix`.
4. If a data-source error appears, download the raw datasets using the provided dataset link.
5. Open Power BI and select:
   `Transform data > Data source settings > Change Source`
6. Connect each query to the corresponding downloaded CSV file.
7. Select `Close & Apply`.
8. Refresh the dashboard.

Power BI Pro is not required to download and open the PBIX file locally in Power BI Desktop.

## Key Insights

- The United States leads the overall athlete-level medal ranking in the dashboard.
- Athletics and swimming are among the leading sports by medals and athlete participation.
- Male athletes represent the larger historical share of participation and medal winners.
- Female Olympic participation shows substantial growth across later Olympic editions.
- Athlete medal success is concentrated across specific sports, countries, and age groups.
- Historical comparisons require careful treatment of country-name and NOC changes.

## Limitations

- Some historical athlete records contain missing demographic values.
- Country names and NOC codes have changed across Olympic history.
- Athlete-level medal records differ from official country medal totals.
- Future Olympic editions in the Games table represent scheduled editions and not completed results.
- The current project primarily provides descriptive and diagnostic analysis.
- Raw data availability depends on the external dataset source link.

## Author

**Ranjeet Anada**

Data Analyst | Excel | SQL | Power BI | Python

[LinkedIn Profile](https://www.linkedin.com/in/ranjeetanada)

## Acknowledgement

This project was developed as part of Data Analytics training at WsCube Tech for educational and portfolio purposes.
