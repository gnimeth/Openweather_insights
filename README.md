
#  Open Weather Insights

- Using Python requests, APIs, and JSON traversals to answer weather related questions.  Project is broken down into two parts.

    - Part 1
        - Create a Python script using citipy and OpenWeatherMap API to visualize the weather of over 500 cities of varying distances from the equator create a representative model of weather across cities.

    - Part 2

        - Using the Geoapify API and the geoViews Python library to create map visualizations


## Dependencies and Setup

```bash
import hvplot.pandas
import pandas as pd
import requests
import matplotlib.pyplot as plt
import numpy as np
import time
import json
from citipy import citipy
from scipy.stats import linregress
```


## Roadmap

- Update .gitignore by adding api keys to the config.py file

#### Part one

- Create Plots to Showcase the Relationship Between Weather Variables and Latitude
![App Screenshot](https://raw.githubusercontent.com/gnimeth/Openweather_insights/main/output_data/Fig1.png)
![App Screenshot](https://raw.githubusercontent.com/gnimeth/Openweather_insights/main/output_data/Fig2.png)
![App Screenshot](https://raw.githubusercontent.com/gnimeth/Openweather_insights/main/output_data/Fig3.png)
![App Screenshot](https://raw.githubusercontent.com/gnimeth/Openweather_insights/main/output_data/Fig4.png)

- Compute Linear Regression for Each Relationship
![App Screenshot](https://raw.githubusercontent.com/gnimeth/Openweather_insights/main/output_data/Screenshot_20230205_035348.png)


#### Part two

- Create a map that displays a point for every city in the city_data_df DataFrame
![App Screenshot](https://raw.githubusercontent.com/gnimeth/Openweather_insights/main/output_data/Screenshot_20230205_034644.png)

-  Narrow down the city_data_df DataFrame to find the ideal weather condition

- For each city in the hotel_df DataFrame, use the Geoapify API to find the first hotel located within 10,000 metres of the coordinates

- Add the hotel name and the country as additional information in the hover message for each city in the map
![App Screenshot](https://raw.githubusercontent.com/gnimeth/Openweather_insights/main/output_data/Screenshot_20230205_034659.png)

## APIs Utilized

- [Geoapify](https://www.geoapify.com/geocoding-api), (2022). 
- [OpenWeather API](https://openweathermap.org/api), (2022). 


