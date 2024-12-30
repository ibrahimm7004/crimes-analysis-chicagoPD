# Chicago Crimes Analysis App

## Live Application
Experience the live app here:
- [Chicago Crimes Analysis App](https://chicago-crimes-analysis.onrender.com)

---

## Overview
This project provides an interactive tool for analyzing crime data from Chicago, using publicly available data from 2010 to 2022. Users can input the name of an area in Chicago to explore detailed visualizations and insights about crime trends and patterns in that area and its surroundings.

The app dynamically generates plots that include:
- A breakdown of the top crimes in the area.
- Monthly and yearly crime trends.
- Arrest status distribution for crimes in the area.

This tool aims to make it easier to understand crime trends and empower communities with data insights.

## Features
- **Interactive Input**: Enter an area name in Chicago to receive visual insights.
- **Custom Visualizations**: Explore crime trends, including crime categories, temporal analysis, and arrest distributions.
- **Proximity Analysis**: View crimes within a 1-kilometer radius of the selected location.

---

## Dataset
The dataset used for this project is publicly available on Kaggle:
- [Crimes in Chicago Dataset (2010-2022)](https://www.kaggle.com/datasets/onlyrohit/crimes-in-chicago/data)

## How It Works
1. The user inputs an area name in the search bar.
2. The app identifies the corresponding latitude and longitude for the area using a lookup CSV.
3. Crimes near the chosen location are filtered and visualized using:
   - Bar charts for top crimes.
   - Line charts for trends over time.
   - Pie charts for arrest status.
4. The user receives three dynamic visualizations to interpret the data.

## Code Summary
The app consists of:
1. **`app.py`**: The main Flask application that handles user input, filters data, and renders visualizations.
2. **`functions.py`**: Contains helper functions for filtering data, calculating nearby areas, and creating plots.
3. **Static CSV Files**:
   - `chicago_areas_avg_coords.csv`: Contains average coordinates for Chicago areas.
   - `final_dataset.csv`: The main crime dataset.

---

## Technologies Used
- **Python**: Backend logic and data manipulation.
- **Flask**: Web framework for handling user interactions.
- **Pandas**: Data filtering and analysis.
- **Plotly**: Generating interactive charts.
- **HTML/CSS**: Frontend design for user interface.

---
