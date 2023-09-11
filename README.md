## Data visualization class project :mag:
By Gabriel Fernandez <br>
Fall 2022 (Updated: Sept. 2023)


## Project bites :chocolate_bar:

**Brief**: Our project centered around analyzing global migration drivers, with a particular focus on World Development Indicators (WDI). Our aim was to extract valuable insights and present them using impactful visualizations.

**Key insights**: Notable findings include a reciprocal migrant flow between Mexico and the USA, the USA remaining a primary destination, and the role of violent conflict in driving migration.

**Tools**: Colab, Python, Tableau 

**Concepts**: ETL (Extract, Transform, Load) and charts (Sankey, Slope, Heatmap, Line, and Scatterplot)


## Project objective :dart:

The United States has more immigrants than any other country, which inspired our group to look into what causes people to migrate across the globe. We looked into factors that included GDP, education, life expectancy, crime rates, climate change, and so forth to understand better why people move. We hope to bring more transparency to the topic of migration. 

## Individual contribution to our data visualization final project

- **Data Preparation and Transformation (ETL)**: I worked on getting our data ready for analysis, involving the extraction, cleaning, transformation, and merging of datasets.

- **Creating Visualizations**: Using Python and Tableau, I crafted charts that helped me better understand the data and discover valuable insights.


### Selected indicators

In our project, I concentrated on two particular indicators to analyze their relationship with migration patterns:

**Internally displaced persons (number of people displaced by conflict and violence)**: This indicator helped me understand the impact of conflict and violence on migration.

**Personal remittances received (% of GDP)**: I selected this indicator to explore the link between remittances and origin countries.


## Datasets


### Dataset 1: UN migrant stock data 

 Table 1: International migrant stock at mid-year by sex and by region, country or area of destination and origin, 1990-2020. The estimates are based on official statistics on the foreign-born or foreign population. This dataset is an Excel file of aggregated statistics. We extracted the country of origin, destination country, and migrant stock for 1990-2020. Source: https://www.un.org/development/desa/pd/content/international-migration-1 
 
### Dataset 2: World development indicators

World Development Indicators (WDI) is the primary World Bank collection of development indicators, compiled from officially recognized international sources. It presents the most current and accurate global development data available and includes national, regional, and global estimates. 
For our presentation, we extracted 47 indicators, 217 countries, and 32 years (1990 - 2021). Then, I combined this data with the migrant stock data to create a master dataset to use in Tableau. Source: https://databank.worldbank.org/source/world-development-indicators

## ETL (Extract, Transform, Load)


For a closer look at our ETL (Extract, Transform, Load) process, you can refer to the Python code available in our Colab notebook: [notebook_documented_ETL](https://colab.research.google.com/drive/1FWbX_sL6De_XxCjx1aOhbMhN-uh7Gp8h?usp=sharing)

<br>

![ETL](images/ETL_diagram.png)

<br>

## Visualizations in Python

### Sankey charts: Show migration flow from origin to destination countries

![Sankey plot 1](images/sankey_chart_1.png)

#### Insights: 

- Mexico is the top source of migrants to the USA, with around 9.5 million total migrants from 1990 to 2020.

<br>
<br>

![Sankey plot 2](images/sankey_chart_2.png)

#### Insights:  
- The USA is Mexico's leading migrant source (0.52 million), yet it receives 19 times more Mexican immigrants than it sends, indicating an immigration imbalance.

<br>
<br>

### Slope charts: Highlight changes between two specific points in time

![Slope chart 1](images/slope_chart_1.png)

#### Insights: 
- The USA has been the primary destination for migrants in 2020 and has held this status since the 1990s.
  
<br>
<br>
 
![Slope chart 2](images/slope_chart_2.png)

#### Insights: 
- Back in 1990, Russia stood at the forefront as the primary supplier of migrants, but as we fast forward to 2020, India had taken over the top position.

<br>
<br>
  
## Visualizations in Tableau

### Heatmap: Displays relationships involving multiple variables
![Heatmap](images/heatmap.png)

#### Insights: 

- The heatmap displays countries with significant immigrant contributions to their populations. It employs size to represent the migrant-to-population ratio and color to indicate remittances as a percentage of GDP. There is an expected correlation between migrant percentages and remittances. However, when sorting by total migrant stock, this association disappears because some countries with large migrant populations also have large overall populations, resulting in a proportionally smaller contribution of remittances to GDP.

<br>
<br>

### Line chart: Depicts general migrant patterns

![Line Chart](images/line_chart.png)

#### Insights: 

- We observe how internal conflicts, like warfare, affect migrant outflows in Syria and Iraq. Conflict onset significantly increases outflows, revealing its profound impact on migration dynamics.
  
<br>
<br>

### Scatterplot: Examines the connection between two variables

![Scatterplot](images/scatterplot.png)

#### Insights: 
- The chart shows the influence of internal conflicts on the number of people leaving a country. Countries like Syria, Afghanistan, and Ukraine have high levels of internal conflict, values above the average reference lines, which has led to many people leaving.

<br>
<br>

## Key insights :bulb:


- Reciprocal Migrant Flow: Mexico is the primary source of US migrants (9.5 average from 1990 to 2020), while the USA significantly contributes to Mexican migration (0.5 million), illustrating a reciprocal dynamic.
  
- Migration Trends: In 2020, the USA continued as the primary destination for migrants since the 90s, while India overtook Russia as the leading migrant source, signifying a significant shift.
  
- Conflict Fuels Migration: War and internal conflict, such as in Syria and Iraq, fuel migrant outflows.

### Lessons learned :sparkles:

- Cross-country migration is a complex and ever-changing phenomenon impacting numerous countries globally. UN estimates, though valuable, may not encompass the complete data due to challenges in data collection, especially when new countries emerge, as seen after the fall of the Soviet Union.

- Given events like the COVID-19 pandemic and emerging conflicts, UN data, reported every five years, may not consistently depict current conditions. I look forward to examining the 2025 data to understand how the pandemic may have influenced global migration patterns.

- Crafting visualization titles that effectively convey the main point demands a blend of trial and error, creativity, and precision.
  
- Tackling the UN's aggregated Excel tables can feel like solving a tricky puzzle. Working to transform them into a more user-friendly long format has been quite the learning adventure.
  






 

