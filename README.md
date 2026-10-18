# World Population Dashboard (R Flexdashboard)

Interactive dashboard for exploring global demographic trends: population, growth, life expectancy,
median age, birth, death and fertility rates, and international migration flows.

## Features

- Key demographic indicators with year, region and country filters
- Time series of natality, mortality and fertility
- Interactive maps of migration flows (Leaflet)
- Interactive tables and CSV export

## Structure

```
world_population_dashboard.Rmd   the dashboard (Flexdashboard + Shiny runtime)
data/data.xlsx                   source data (sheet "Reel")
assets/                          logo and favicon
```

## Run it

```r
install.packages(c("flexdashboard", "shiny", "dplyr", "plotly", "highcharter", "DT",
                   "readxl", "leaflet", "rnaturalearth", "sf", "countrycode"))
rmarkdown::run("world_population_dashboard.Rmd")
```

Or open the `.Rproj` in RStudio and click **Run Document**.

**Author:** Klaus KUEKOU · [LinkedIn](https://www.linkedin.com/in/klaus-kuekou-217bba173)
