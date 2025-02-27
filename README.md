# Suicide-Rates-Data-Visualization
This project visualizes global suicide rates using a dataset spanning from 1985 to 2016. The visualization provides insights into global suicide trends based on factors such as age, gender, continent, and country. 
The dashboard is created using the flexdashboard package in R and includes interactive plots, value boxes, and tables to make data exploration easier and more engaging.

---
# **Project Overview**

The dashboard is divided into two main sections:
1. By World & Continent

  * Overall Trend: Displays the global trend of suicides per 100K population from 1985 to 2016.
  * By Age: Shows suicide rates by different age groups over time.
  * By Gender: Visualizes suicide rates by gender across years.
  * Suicides by Continent and Gender: Displays suicide rates for different continents, broken down by gender.
  * Suicides by Continent and Age: Shows suicide rates by continent, segmented by age group.
  * Global Suicide Rate: Displays a key value for the overall suicide rate globally.

2. By Country

  * Suicides by Country: Presents a bar chart showing suicide rates by country, allowing for easy comparison.

# **Technologies Used**

  * R: Programming language used to manipulate data and create visualizations.
  * flexdashboard: A package that creates interactive dashboards.
  * highcharter: A library for interactive charts based on Highcharts.
  * plotly: Another library for creating interactive visualizations.
  * viridis: A color palette package for better color schemes.
  * tidyverse: A collection of R packages for data manipulation.
  * countrycode: A package for converting country names to continent names.
  * DT: A package for displaying interactive data tables.
  * rjson and crosstalk: Used for working with JSON data and interactive features in the dashboard.

# **Setup**

* Install Required Packages To run the project, you need to install the following R packages:

   install.packages(c("flexdashboard", "knitr", "highcharter", "plotly", "viridis", 
                   "tidyverse", "countrycode", "rjson", "crosstalk", "DT"))

* Load Data The dataset is stored in master.csv, which contains information on suicides across various countries, categorized by year, age, sex, and population. This dataset is read into the R environment using:

   data <- read.csv('master.csv')

* Customize Theme A custom theme for highcharts is defined to enhance the visual appeal of the charts:

  custom_theme <- hc_theme(
      colors = c('#D664BE', 'blue', 'pink'),
      chart = list(backgroundColor = '#FAFAFA', plotBorderColor = "black"),
      ...
    )

# **Features and Visualizations**

* Overall Suicide Trends
  Line plots to show global suicide rates by year, segmented by age and gender.

* Regional Analysis
  Suicides by continent and gender, and by continent and age, are visualized using column charts for better regional insights.

* Country-Level Insights
  An interactive bar chart visualizes suicide rates by country, ranked by the highest suicide rates.

* Key Metrics
  Value boxes to display key statistics, such as the overall global suicide rate per 100K population.

# **References**

  * Kaggle 2018, "Suicide Rates Overview 1985 to 2016," viewed 22 October 2021, Kaggle.
  * United Nations Development Program. (2018). Human Development Index (HDI). UNDP
  * World Health Organization (2018). Suicide prevention. WHO

# **Usage**

To run the visualization, open the RMarkdown file in RStudio and execute it. The dashboard will render an interactive visualization of suicide rates based on different factors.
