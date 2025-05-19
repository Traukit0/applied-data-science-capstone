# SpaceX Falcon 9 First Stage Landing Prediction

## Summary

This capstone project predicts if the SpaceX Falcon 9 first stage will land successfully.

The full report can be found [here](IBM%20Data%20Science%20Capstone%20Project.pdf). 

## Context and Business Understanding

SpaceX launches Falcon 9 rockets at a cost of around $62m. This is considerably cheaper than other providers (which usually cost upwards of $165m), and much of the savings are because SpaceX can land, and then re-use the first stage of the rocket.

If we can make predictions on whether the first stage will land, we can determine the cost of a launch, and use this information to assess whether or not an alternate company should bid against SpaceX for a rocket launch.

## 📑 Main Topics

This project follows these steps:

### Data Collection
* Making GET requests to the SpaceX REST API
* Web Scraping

### Data Wrangling
* Using the `.fillna()` method to remove NaN values
* Using the `.value_counts()` method to determine the following:
    * Number of launches on each site
    * Number and occurrence of each orbit
    * Number and occurrence of mission outcome per orbit type
* Creating a landing outcome label that shows the following:
    * 0 when the booster did not land successfully
    * 1 when the booster did land successfully

### Exploratory Data Analysis
* Using SQL queries to manipulate and evaluate the SpaceX dataset
* Using Pandas and Matplotlib to visualize relationships between variables, and determine patterns

### Interactive Visual Analytics
* Geospatial analytics using Folium
* Creating an interactive dashboard using Plotly Dash

### Predictive Analysis (Classification)
* Using Scikit-Learn to:
    * Pre-process (standardize) the data
    * Split the data into training and testing data using `train_test_split`
    * Train different classification models
    * Find hyperparameters using `GridSearchCV`
    * Plotting confusion matrices for each classification model
    * Assessing the accuracy of each classification model

## 🔑 Key Skills Learned/Used
* Using data science methodologies to define and formulate a real-world business problem
* Using data analysis and data visualisation to load a dataset, clean it, and find out interesting insights from it
* Interactive dashboard development with Plotly Dash
* Interactive map development using Folium
* Using machine learning to build a predictive model to help a business function more efficiently
* Structuring and building a data-findings report

## Project Files

*   `01 - jupyter-labs-spacex-data-collection-api.ipynb`: Jupyter Notebook for data collection using the SpaceX API.
*   `02 - jupyter-labs-webscraping.ipynb`: Jupyter Notebook for web scraping additional data.
*   `03 - labs-jupyter-spacex-Data wrangling.ipynb`: Jupyter Notebook for data wrangling and cleaning.
*   `04 - jupyter-labs-eda-sql-coursera_sqllite.ipynb`: Jupyter Notebook for exploratory data analysis using SQL.
*   `05 - edadataviz.ipynb`: Jupyter Notebook for exploratory data analysis and visualization.
*   `06 - lab_jupyter_launch_site_location.ipynb`: Jupyter Notebook for geospatial analysis of launch sites.
*   `07 - SpaceX_Machine Learning Prediction_Part_5.ipynb`: Jupyter Notebook for building and evaluating machine learning models.
*   `spacex_dash_app.py`: Python script for the Plotly Dash interactive dashboard.
*   `IBM Data Science Capstone Project.pdf`: The main project report.
*   `IBM Data Science Capstone Project.pptx` and `IBM Data Science Capstone Project 2022.pptx`: Project presentations.
*   `.gitignore`: Specifies intentionally untracked files that Git should ignore. 