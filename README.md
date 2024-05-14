![Colorful infographic illustrating various Airbnb data metrics for New York City, including rental statistics, neighborhood distribution, and review counts, presented in a stylized cityscape with charts and graphs](./Images/Airbnb%20Graphic.webp)

# Airbnb New York City Listings Data Visualization

## Table of Contents

1. [Overview](#overview)
2. [Graph Descriptions](#graph-descriptions)
   - [Listings by Room Type](#1-listings-by-room-type)
   - [Neighborhoods Word Cloud](#2-neighborhoods-word-cloud)
   - [Reviews per Borough](#3-reviews-per-borough)
   - [Scatter Plot and Map of Listings](#4-scatter-plot-and-map-of-listings)
   - [Map of Airbnb Listings by Neighborhood Group](#5-map-of-airbnb-listings-by-neighborhood-group)
3. [Data Source](#data-source)
4. [Conclusion](#conclusion)

# Airbnb New York City Listings Data Visualization

## Overview

This document provides a detailed description of the data visualizations related to Airbnb listings in New York City, captured in several graphs.

## Graph Descriptions

### 1. Scatter Plot and Map of Listings

![Scatter Plot 1](./Images/Vadim%20-%20Scatter%20Plot%20of%20NYC.png)
![Scatter Plot 2](./Images/Vadim%20-%20Scatter%20Plot%20+%20Map.png)

- **Description**: These visualizations combine a scatter plot and a map, marking the geographical distribution of Airbnb listings across New York City's boroughs.

### 2. Neighborhoods Word Cloud

![Neighborhoods Word Cloud](./Images/Vadim%20-%20Neighberhoods%20Word%20Cloud.png)

- **Description**: A word cloud highlighting the most popular neighborhoods for Airbnb listings in New York City.
- **Features**: The size of each neighborhood's name indicates its frequency or popularity among listings. Major neighborhoods like "East Village", "Williamsburg", and "Harlem" appear prominently.

### 3. Reviews per Borough

![Reviews per Borough](./Images/Vadim%20-%20Reviews%20per%20Borough.png)

- **Description**: A pie chart showing the percentage distribution of reviews across different boroughs of New York City.
- **Boroughs**:
  - Manhattan: Holds the largest share of reviews, indicative of high visitor engagement.
  - Brooklyn: Follows closely, suggesting it's also a popular choice for Airbnb users.
  - Queens, Bronx, Staten Island: These areas have fewer reviews compared to Manhattan and Brooklyn.

### 4. Listings by Room Type

![Listings by Room Type](./Images/Vadim%20-%20Listings%20by%20Room%20Type.png)

- **Description**: This bar chart illustrates the distribution of Airbnb listings by room type.
- **Types**:
  - Entire home/apt: Represents listings where guests have the entire property to themselves.
  - Private room: Indicates listings that offer private rooms within a shared property.
  - Hotel room: Includes listings categorized under the traditional hotel room setup.
  - Shared room: Listings where the space is shared with other guests.

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

## Data Source

The data used in these visualizations are sourced from Airbnb's publicly available datasets.

## Conclusion

These visualizations offer valuable insights into the Airbnb rental landscape in New York City, helping to understand trends, guest preferences, and geographical demand distribution.
