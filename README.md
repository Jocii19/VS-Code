# Taxi & Weather ETL Pipeline 🚕





## Project Overview 📌

This repository contains an ETL (Extract – Transform – Load) pipeline implemented in a Jupyter Notebook. The project processes taxi trip data and weather data, performs data cleaning and transformation, builds dimension tables, and prepares the data for analytical or database loading purposes.

The main goal is to demonstrate a clean data transformation & loading workflow using Python and pandas.







## Data Description 🗂️


### Taxi Data 🚕

The taxi dataset is transformed into a star-schema–like structure:

° Fact table: taxi trips

° Dimension tables:

      ° Company dimension

      ° Payment type dimension

Each dimension is assigned a unique identifier, which is referenced from the fact table.


### Weather Data 🌦️

Weather data is transformed separately to:

° standardize formats,

° align timestamps with taxi trips,

° enable analytical joins and aggregations.



## Tech Stack 🛠️

° Python 3

° Jupyter Notebook

° pandas

° requests

° python-dateutil

```python
📁 Project Structure
├── 07_transform_load.ipynb   # Transform & Load ETL notebook
└── README.md                # Project documentation
```



## ETL Workflow 🔄

1.Environment setup and library imports

2.Data ingestion

3.Data cleaning and preprocessing

4.Dimension table creation (Company, Payment)

5.Weather data transformation

6.Data preparation for loading



## How to Run ▶️
Prerequisites

° Python 3.x

° Jupyter Notebook

Installation
```python
pip install pandas requests python-dateutil
```
Execution
```python
jupyter notebook 07_transform_load.ipynb
```

Run all cells sequentially.


## Output 📤

After execution, the notebook produces:

° normalized dimension tables,

° clean and structured fact data,

° datasets ready for database loading or BI analysis.



## Notes 📌

° This project is intended for educational and demonstration purposes

° Easily extendable with additional dimensions or data sources



 ## License 📄

This project is available for free use for educational and non-commercial purposes.
