# Election Results Analysis

This project aims to develop a model that detects the most representative polling units in local elections. The model is designed to predict election outcomes with high accuracy by focusing on historical election data and identifying key neighborhoods.

## Overview

The main goal of this project is to address the absence of a model that accurately and affordably finds the most representative neighborhoods in a given city. Analyzing the election results of these selected neighborhoods provides a highly accurate overview of the future election outcomes.

## Features

- **Data Scraping:** Collects past election results from 2014 and 2019.
- **Mixed-Integer Programming (MIP):** Detects the most representative neighborhoods and their weight coefficients using scraped data.
- **High Accuracy:** The model demonstrates a weighted absolute error value of less than 10% for each test case.
- **Optimization:** Enhances prediction accuracy by minimizing Euclidean distance in multi-dimensional space.

## Methodology

1. **Data Scraping:**
   - Python scripts using Selenium to automate the process of downloading election data from the Supreme Election Council of Turkey (YSK) website.
   - Data cleansing and aggregation to prepare datasets for modeling.

2. **Modeling:**
   - Creation of a Mixed-Integer Program (MIP) to select the most representative neighborhoods.
   - Calculation of weight coefficients for the selected neighborhoods to maximize the accuracy function.

3. **Testing:**
   - Validation of the model using the results of the 2024 metropolitan municipality elections.
   - Analysis of prediction accuracy and error metrics.

## Technologies Used

- **Programming Languages:** Python
- **Libraries:** Selenium, Pandas, NumPy
- **Optimization Tools:** Gurobi Optimizer

## Getting Started

### Prerequisites

- Python 3.7 or higher
- Selenium
- Pandas
- NumPy
- Gurobi Optimizer (with a valid license)

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/election-results-analysis.git
   cd election-results-analysis
