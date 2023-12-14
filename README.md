# Intel Lab Data Analysis Project

## Overview
Hello There! In this project, I analyzed a dataset provided by the Intel Berkeley Research lab. The dataset collected information from 54 sensors between February 28th and April 5th, 2004.

## Dataset

- **Source:** [Intel Berkeley Research Lab Data](https://db.csail.mit.edu/labdata/labdata.html)
- **Size:** 34MB gzipped, 150MB uncompressed
- **Schema:**
  - date: yyyy-mm-dd
  - time: hh:mm:ss.xxx
  - epoch: int
  - moteid: int
  - temperature: real
  - humidity: real
  - light: real
  - voltage: real

## Analysis Tools

The analysis was performed using Python with the following libraries:

- [Pandas](https://pandas.pydata.org/) for data manipulation.
- [Matplotlib](https://matplotlib.org/) for basic data visualization.
- [Seaborn](https://seaborn.pydata.org/) for statistical data visualization using Matplotlib as base.

## Data Processing

The dataset was processed to handle missing values and explore patterns in temperature, humidity, light, and voltage over time. Visualization using seaborn for easier representation of the data effectively.

## Heat Index and Brightness Analysis

The heat Index was calculated using the recommended formula by NWS.
- Brightness levels were analyzed with specific sectors identified:
  - 0 - 200 lux: Minimal light, similar to moonlight or very low artificial lighting.
  - 200 - 400 lux: Twilight or minimal street lighting.
  - 400 - 600 lux: Comparable to bright office lighting or sunrise/sunset conditions.
  - 600 - 800 lux: Adequate for various indoor activities, such as reading or working.
  - 800 - 1000 lux: Bright lighting conditions suitable for tasks requiring high visibility in the lab.

## Conclusion

Key findings include:

- Temperature influences brightness levels.
- Some data cleaning is required from the source.
- Comfortable temperature levels were generally maintained in the lab, with occasional anomalies.

## Project Execution

The project was executed using Jupyter Notebook with the following steps:

1. Data download using `wget` from [Intel Lab Data](https://db.csail.mit.edu/labdata/labdata.html).
2. Conversion of data to a DataFrame using Pandas.
3. Data cleaning to handle missing values and ensure data integrity.
4. Heat Index calculation and integration into the DataFrame.
5. Grouping and visualization of data patterns.
6. Heatmap creation to visualize distributions over time.

Feel free to explore the project 🌟

