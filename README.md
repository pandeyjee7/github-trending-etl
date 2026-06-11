
# GitHub Trending Repositories ETL Pipeline

A lightweight, beginner-friendly ETL (Extract, Transform, Load) pipeline that automates data collection from the GitHub API, processes it for data quality, and outputs a clean dataset.

## Project Architecture



The project follows standard data engineering principles:
1. **Extract**: Dynamically calculates the date from 30 days ago and queries the GitHub REST API for top repositories sorted by stars.
2. **Transform**: Uses Python and `pandas` to filter out unstructured JSON metadata, handles missing values (e.g., classifying blank coding languages as "Unknown"), and formats data structures.
3. **Load**: Exports the processed, structured table into a local `trending_github_repositories.csv` file.

## Tech Stack & Core Concepts
* **Language:** Python 3.x
* **Libraries:** `requests` (Data Extraction), `pandas` (Data Manipulation & Cleaning), `datetime` (Dynamic filtering)
* **Environment:** Google Colab / Jupyter Notebooks
* **Data Engineering Concepts:** API Integration, Data Schema Filtering, Data Transformation, Handling Missing/Null Values.

## How to Run
1. Open the `.ipynb` notebook file in Google Colab or any Jupyter environment.
2. Run the cells sequentially from top to bottom.
3. Download the generated `trending_github_repositories.csv` file from the environment's file explorer.
