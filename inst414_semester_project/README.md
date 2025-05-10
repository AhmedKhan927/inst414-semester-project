# INST414_Semester_Project

<a target="_blank" href="https://cookiecutter-data-science.drivendata.org/">
    <img src="https://img.shields.io/badge/CCDS-Project%20template-328F97?logo=cookiecutter" />
</a>
Author: Ahmed Khan
Course: INST414
Semester: Spring 2025

## Overview
This project investigates the impact of remote work on employee work-life balance and productivity. It uses survey data from the New South Wales (NSW) government's 2020 Remote Work Survey, analyzing changes in personal time, commute time, and self-reported productivity between remote work and in-office work settings.

## Research Questions
1. Does remote work significantly improve work-life balance compared to in-office work?
2. What factors predict productivity during remote work?

## Dataset
Source: Kaggle (NSW Government Remote Work Survey)
Sample Size: 1507 Responses
Sample Size After Cleaning: 899

Features Used:
- Time spent remote vs. in-office
- Self-reported productivity
- Commute and prep time
- Collaboration ease
- Preference for remote work

   

## Project Organization

```
├── LICENSE            <- Open-source license if one is chosen
├── Makefile           <- Makefile with convenience commands like `make data` or `make train`
├── README.md          <- The top-level README for developers using this project.
├── data
│   ├── external       <- Data from third party sources.
│   ├── interim        <- Intermediate data that has been transformed.
│   ├── processed      <- The final, canonical data sets for modeling.
│   └── raw            <- The original, immutable data dump.
│
├── docs               <- A default mkdocs project; see www.mkdocs.org for details
│
├── models             <- Trained and serialized models, model predictions, or model summaries
│
├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
│                         the creator's initials, and a short `-` delimited description, e.g.
│                         `1.0-jqp-initial-data-exploration`.
│
├── pyproject.toml     <- Project configuration file with package metadata for 
│                         inst414_semester_project and configuration for tools like black
│
├── references         <- Data dictionaries, manuals, and all other explanatory materials.
│
├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
│   └── figures        <- Generated graphics and figures to be used in reporting
│
├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
│                         generated with `pip freeze > requirements.txt`
│
├── setup.cfg          <- Configuration file for flake8
│
└── inst414_semester_project   <- Source code for use in this project.
    │
    ├── __init__.py             <- Makes inst414_semester_project a Python module
    │
    ├── config.py               <- Store useful variables and configuration
    │
    ├── dataset.py              <- Scripts to download or generate data
    │
    ├── features.py             <- Code to create features for modeling
    │
    ├── modeling                
    │   ├── __init__.py 
    │   ├── predict.py          <- Code to run model inference with trained models          
    │   └── train.py            <- Code to train models
    │
    └── plots.py                <- Code to create visualizations
```

--------

## Methods used
- Data Cleaning (null values, outliers, column renaming)
- Exploratory Data Analysis, EDA (Boxplots, histograms, summary statistics)
- Sign Test (non-parametric hypothesis testing)
- Multiple Linear Regression (Predicting productivity from remote work factors)

## How to replicate the pipeline

1. Clone the repository
```bash
git clone https://github.com/AhmedKhan927/inst414-semester-project.git
cd inst414-semester-project
```
2. Create and activate a virtual environment

```bash
python -m venv venv
source venv/bin/activate
```

3. Install packages

```bash
pip install -r requirements.txt
```
4. Launch a fresh Jupyter Notebook
5. Follow the code cells in the notebooks folder to run the analysis and generate results.

## Key Findings
- Personal time significantly increases on remote workdays compared to in-office days.
- Ease of collaboration is the strongest predictor of perceived productivity during remote work.
- Employees save an average of 1.2 hours per day in prep and commute time when working remotely

Documentation:
See INST414 Research Project.pdf in docs/docs