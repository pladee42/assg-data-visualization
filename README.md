# Data Science Assignment 1: Data Visualization

## Overview
This project aims to analyze carbon emissions data from the dataset `owid-co2-data.csv`. The analysis explores several questions related to the growth of CO₂ emissions, their relationship with GDP, and wealth inequality over time. It involves plotting various trends, comparing different regions, and annotating key data points for deeper insights.

## Dataset
The dataset used for the analysis is `owid-co2-data.csv`, which contains CO₂ emissions data across different countries and years.

### Data Columns:
- **country**: Name of the country
- **year**: Year of data point
- **co2**: Total CO₂ emissions in million tonnes
- **co2_per_capita**: CO₂ emissions per capita (in tonnes)
- **gdp**: Gross Domestic Product of the country
- **population**: Population of the country
- **iso_code**: ISO country code
- etc.

## Installation
Ensure you have the following libraries installed:
- pandas
- numpy
- matplotlib
- seaborn

You can create a conda environment from the `com6018.environment.yml` file and activate it,

```bash
cd assg-data-visualization
conda env create -n com6018 -f com6018.environment.yml
conda activate com6018
```

## Assignment Questions and Solutions

### Q1. The Growth of CO₂ Emissions
This question analyzes the growth of CO₂ emissions across continents (Africa, Asia, Europe, North America, Oceania, South America) from 1950 to 2021. We plot:
1. Total annual CO₂ emissions for each continent.
2. Per capita CO₂ emissions for each continent.

The code creates two line plots to illustrate these trends and compares the relative contributions of each continent in terms of total emissions and per capita emissions.

#### Key Findings:
- Asia had the highest total CO₂ emissions, but its per capita emissions ranked fourth.
- Oceania had the lowest total emissions but one of the highest per capita emissions.

### Q2. The Share of CO₂ Emissions by Country Over Time
In this section, we look at the five countries with the highest CO₂ emissions in 2020. We analyze their share of global and European emissions in 1960, 1990, and 2020, represented as pie charts.

#### Key Findings:
- The top global emitters have increased their share of total emissions, growing from 52.5% in 1960 to nearly 60% in 2020.
- Similarly, the top European producers grew their share from 60.8% in 1960 to 66.1% in 2020.

### Q3. The Link Between GDP and CO₂ Emissions
This part examines whether countries with high GDP also have high per capita CO₂ emissions. The plot shows the relationship between GDP per capita and CO₂ per capita for countries with populations greater than 10 million in 1978, 1998, and 2018.

#### Key Findings:
- Many countries have reduced CO₂ emissions per capita relative to their economic growth.
- Countries like China, South Korea, and Saudi Arabia show a closer link between GDP growth and higher CO₂ emissions.

### Q4. The Development of Wealth Inequality Over Time
This section investigates the distribution of GDP per capita from 1950 to 2020, focusing on countries with populations of at least 5 million in 2020. We highlight the World Bank poverty threshold (GDP per capita < 785 USD) and track the number of people living in poverty over time.

#### Key Findings:
- The number of people living below the poverty threshold has grown, although as a proportion of the world's total population, it has varied.

## How to Use
1. Clone or download this repository.
2. Place the `owid-co2-data.csv` file in the same directory as the notebook.
3. Run the notebook cells sequentially to load the data, generate plots, and analyze the results.
