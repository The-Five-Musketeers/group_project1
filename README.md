![Colorful infographic illustrating various Airbnb data metrics for New York City, including rental statistics, neighborhood distribution, and review counts, presented in a stylized cityscape with charts and graphs](./Images/Airbnb%20Graphic.webp)

# Airbnb New York City Listings Data Visualization

## Table of Contents

1. [Overview](#overview)
2. [Installation](#installation)
   - [Importing Libraries](#importing-libraries)
3. [Graph Descriptions](#graph-descriptions)
   - [Scatter Plot and Map of Listings](#1-scatter-plot-and-map-of-listings)
   - [Neighborhoods Word Cloud](#2-neighborhoods-word-cloud)
   - [Reviews per Borough](#3-reviews-per-borough)
   - [Listings by Room Type](#4-listings-by-room-type)
   - [Listings by Neighborhoods](#5-listings-by-neighborhoods)
   - [Listings by Boroughs](#6-listings-by-boroughs)
   - [Average Price By Borough](#7-average-price-by-borough)
   - [Average Price By Neighborhood](#8-average-price-by-neighborhood)
   - [Average Price By Top 5 Neighborhood over Time](#9-average-price-by-top-5-neighborhood-over-time)
4. [Data Source](#data-source)
5. [Conclusion](#conclusion)

## Overview

This document provides a detailed description of the data visualizations related to Airbnb listings in New York City, captured in several graphs.

## Installation

To reproduce the visualizations in this project, you will need to install the following Python libraries:

```bash
pip install pandas matplotlib numpy seaborn plotly python-dotenv wordcloud
```

### Importing Libraries

Ensure you import the following libraries in your Python script:

```python
import pandas as pd
import matplotlib.pyplot as plt
import numpy as np
import seaborn as sns
import plotly.express as px
import os
from dotenv import load_dotenv
from wordcloud import WordCloud
import datetime as dt
```

## Graph Descriptions

### 1. Scatter Plot and Map of Listings

![Scatter Plot 1](./Images/Vadim%20-%20Scatter%20Plot%20of%20NYC.png)
![Scatter Plot 2](./Images/Vadim%20-%20Scatter%20Plot%20+%20Map.png)

- **Description**: These visualizations combine a scatter plot and a map, marking the geographical distribution of Airbnb listings across New York City's boroughs.

### 2. Neighborhoods Word Cloud

![Neighborhoods Word Cloud](./Images/Vadim%20-%20Neighberhoods%20Word%20Cloud.png)

- **Description**: A word cloud highlighting the most popular neighborhoods for Airbnb listings in New York City.
- **Features**: The size of each neighborhood's name indicates its frequency or popularity among listings. Major neighborhoods like "East Village", "Williamsburg", "Bedford Stuyvesant", and "Harlem" appear prominently.

### 3. Reviews per Borough

![Reviews per Borough](./Images/Vadim%20-%20Reviews%20per%20Borough.png)

- **Description**: A pie chart showing the percentage distribution of reviews across different boroughs of New York City.
- **Brooklyn Leads in Reviews:**
- Despite Manhattan having more listings, Brooklyn has the highest share of reviews at 42.6%. This suggests that guests in Brooklyn might be more engaged in providing feedback, or that the average length of stay and interaction level in Brooklyn listings is higher.

**Manhattan’s Lower Review Share:**

- Manhattan, with a higher number of listings, has 32.3% of the reviews. This could indicate several factors:
  Shorter Stays: Visitors to Manhattan might stay for shorter durations, reducing the likelihood of leaving reviews.
  Higher Turnover: The high turnover rate in Manhattan's listings might result in fewer reviews per listing.
  Different Guest Demographics: Guests in Manhattan might be less inclined to leave reviews, possibly due to a higher proportion of business travelers.

### 4. Listings by Room Type

![Listings by Room Type](./Images/Vadim%20-%20Listings%20by%20Room%20Type.png)

- **Description**: This bar chart illustrates the distribution of Airbnb listings by room type.
- **High Demand for Entire Homes/Apartments:**

**Tourism and Business Travel:** The high number of entire homes/apartments indicates a strong demand from tourists and business travelers who prefer the privacy and convenience of having an entire place to themselves.
Impact on Housing Market: The significant number of entire homes/apartments being used for short-term rentals might reduce the availability of long-term rental properties, potentially driving up rental prices for residents.
Significant Market for Private Rooms:

**Affordable Options:** Private room listings provide more affordable accommodation options for travelers, which can attract budget-conscious tourists and younger visitors.

**Income for Residents:** This also suggests that many city residents are using Airbnb to supplement their income by renting out spare rooms.

### 5. Listings by Neighborhoods

![Listings by Neighborhoods](./Images/Ramona%20%20-%20Listing%20by%20Neighborhood.png)

- **Description**: This bar chart illustrates the distribution of Airbnb listings by neighborhoods.
- **Types**:
- X-axis: Represents different neighborhoods in New York City.
- Y-axis: Indicates the total number of unique Airbnb listings in each neighborhood.
- Midtown, Upper East Side, and Murray Hill show a high concentration of listings, each with over 700 unique properties. This suggests these areas are highly popular with Airbnb hosts, possibly due to their central location and tourist attractions.
- Theater District and Hell's Kitchen also display a significant number of listings, highlighting their appeal, likely driven by their proximity to entertainment and dining options.
- Bushwick shows fewer listings compared to other neighborhoods, indicating either a lower demand or lesser development of Airbnb market penetration in this area

### 6. Listings by Boroughs

![Listings by Borough](./Images/Ramona%20-%20Listing%20by%20Borough.png)

- **Description**: This bar chart illustrates the distribution of Airbnb listings by neighborhoods.
- **Types**:
- X-axis: Represents the five boroughs of New York City — Manhattan, Brooklyn, Queens, Bronx, and Staten Island.
- Y-axis: Indicates the total number of unique Airbnb listings in each borough.
- Manhattan has the highest number of listings, significantly outpacing the other boroughs with over 2500 unique listings. This is likely due to its status as a major tourist and business hub.
- Brooklyn and Queens show moderate activity, each hosting over 1000 listings. These boroughs are popular among visitors seeking a more residential atmosphere while still being accessible to Manhattan.
- The Bronx and Staten Island have considerably fewer listings, suggesting lower tourist traffic and potentially stricter local regulations or lesser demand.

### 7. Average Price By Borough

![Listings by Borough](./Images/Danny_Avg%20Price%20per%20Borough.png)

- **Description**: This bar chart illustrates the median price of NYC Airbnb listings by Borough.
- **Types**:
- X-axis: Represents the five boroughs of New York City — Manhattan, Brooklyn, Queens, Bronx, and Staten Island.
- Y-axis: Indicates the avg price of Airbnb listings in each borough.
- Manhattan had the highest avg price on listings.
- Brookyln and Staten Island follow.

### 8. Average Price By Neighborhood

![Listings by Borough](./Images/Danny_Top%205%20Average%20Price%20per%20Neighborhood.png)

- **Description**: This bar chart illustrates the median price of top 5 NYC Airbnb listings by Neighborhood.
- **Types**:
- X-axis: Represents the top five neigborhoods of New York City based on our data.
- Y-axis: Indicates the avg price of Airbnb listings in each neighborhood.
- Tribeca and Soho had the highest avg price
- DUMBO in Brooklyn rounds out the top 5

### 9. Average Price By Top 5 Neighborhood over Time

![Listings by Borough](./Images/Danny_AirBnB_Price_by_Top_5_Neighborhood_Over_Time.png)

- **Description**: This line graph illustrates the median price of top 5 NYC Airbnb listings by Neighborhood over time. This is meant to dive deeper into the price trends we are seeing month over month across the available years.
- **Types**:
- X-axis: Represents the top five neigborhoods of New York City based on our data.
- Y-axis: Indicates the avg price of Airbnb listings in each neighborhood over time.
- The data suggests a downard trend in pricing beginning in January of 2024, but more data is needed to see if this is a predicatble trend.

## Data Source

The data used in these visualizations are sourced from Airbnb's publicly available datasets:
[Airbnb's publicly available datasets](https://insideairbnb.com/get-the-data/)

## Conclusion

These visualizations offer valuable insights into the Airbnb rental landscape in New York City, helping to understand trends, guest preferences, and geographical demand distribution.
