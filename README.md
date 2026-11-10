# Netflix Content Analysis Dashboard | Power BI

## Project Overview

The **Netflix Content Analysis Dashboard** is an interactive Power BI project designed to explore Netflix's content catalog. It provides an overview of movies and TV shows and helps users examine content distribution across release years, ratings, and countries.

The dashboard brings key content metrics and visual analysis together in one place, with slicers that allow users to explore the data based on selected criteria.

## Dashboard Preview

> Add a screenshot of your Power BI dashboard to this repository and replace the placeholder below.

![Netflix Content Analysis Dashboard](images/netflix-dashboard.png)

## Key Features

- **KPI Cards:** Display total shows, movies, and TV shows.
- **Content Type Analysis:** Compare the distribution of movies and TV shows.
- **Release Year Analysis:** Explore the number of titles by release year.
- **Rating Analysis:** Examine content distribution across ratings.
- **Country Analysis:** Explore the geographic distribution of Netflix titles.
- **Interactive Filters:** Filter the report by country, release year, and show type.

## Tools and Technologies

- **Microsoft Power BI Desktop** – Dashboard development and data visualization
- **Power Query** – Data preparation and transformation (where applied)
- **DAX** – Measures used for report KPIs
- **Data Visualization** – KPI cards, donut charts, area chart, column chart, and map

## Data Fields Used

The report references fields from the `netflix_titles` table, including:

- `show_id`
- `type`
- `release_year`
- `rating`
- `country`
- `director`

The KPI cards use measures named `Total shows`, `Movies`, and `TV Shows` from the `mesure_` table.

## Dashboard Insights

The dashboard is designed to help answer questions such as:

1. How many titles are included in the catalog?
2. How does the catalog compare movies with TV shows?
3. How has the number of titles changed across release years?
4. Which content ratings appear in the catalog?
5. How is content distributed across countries?
6. How do the results change when users select a country, year, or content type?

> Add numerical findings only after validating the values in the report. This README does not claim specific totals or trends because those values have not been independently verified.

## How to Use

1. Download or clone this repository.
2. Open `Netflix Content DashBoard.pbix` using Microsoft Power BI Desktop.
3. Wait for the report to load.
4. Use the country, release year, and show type slicers to filter the visuals.
5. Select chart elements to explore the report interactively.

## Repository Structure

```text
Netflix-Content-Analysis/
│
├── Netflix Content DashBoard.pbix
├── README.md
└── images/
    └── netflix-dashboard.png
```

The `images/netflix-dashboard.png` file is a suggested screenshot location. Add your own dashboard screenshot to the `images` folder.

## Validation Note

The report contains a second donut chart grouped by `type` that currently aggregates `director` using a count. This counts non-empty director values, not all titles. If the intended metric is the number of titles by content type, use a count of `show_id` instead.

Also validate how multiple countries per title and missing values are handled before interpreting country-level results.

## Future Improvements

- Add verified analytical findings to the dashboard and this README.
- Review missing values in fields such as `director`, `country`, and `rating`.
- Use a consistent title-count measure across content-type visuals.
- Improve chart titles and labels so each metric is immediately clear.
- Add a dashboard screenshot and, if available, a short demonstration.

## Author

**Prashanth**  
MCA Graduate | Aspiring Data Analyst | Power BI

---

*This project was created for learning and portfolio demonstration purposes.*
