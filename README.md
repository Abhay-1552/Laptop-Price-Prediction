# Laptop Price Prediction

This repository contains the project "Laptop Price Prediction," where we scrape laptop data from Flipkart, clean and analyze the data, and then build a machine learning model to predict laptop prices. The entire project is divided into several stages, including data scraping, cleaning, exploratory data analysis (EDA), model building, and creating a frontend using Streamlit for visualization.

## Table of Contents
- [Data Scraping](#data-scraping)
- [Data Cleaning and Analysis](#data-cleaning-and-analysis)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Model Building](#model-building)
- [Model Evaluation](#model-evaluation)
- [Pickle File Creation](#pickle-file-creation)
- [Frontend with Streamlit](#frontend-with-streamlit)
- [Links](#links)
- [Installation](#installation)
- [Usage](#usage)

## Data Scraping

We scrape the laptop data from Flipkart using BeautifulSoup. The code for data scraping is available in another repository. You can find the code [here](https://github.com/your-repo/data-scraping-repo).

## Data Cleaning and Analysis

After scraping the data, we perform cleaning and analysis using Pandas, NumPy, and regular expressions (re). The data is prepared for further analysis and modeling.

## Exploratory Data Analysis (EDA)

We conduct EDA using Matplotlib and Seaborn to visualize and understand the patterns and distributions in the data.

## Model Building

For the model building, we split the data into training and testing sets and created a model pipeline.

- **ColumnTransformer**: Applies One-Hot Encoding to categorical features.
- **LinearRegression, RandomForestRegressor, GradientBoostingRegressor**: Different regression models used for prediction.
- **VotingRegressor**: Combines predictions from multiple models.
- **Pipeline**: Streamlines the workflow by combining preprocessing and model steps.

## Model Evaluation

We evaluate the model using cross-validation and calculate metrics such as R2 score and Mean Absolute Error (MAE).

## Pickle File Creation

The final model and data are saved into a pickle file for future use.

## Frontend with Streamlit

A frontend is created using Streamlit for visual presentation and interaction with the model.

## Links

- [Data Scraping Repository](https://github.com/your-repo/data-scraping-repo)

## Installation

To run this project, follow these steps:

1. Clone the repository.
   ```sh
   git clone https://github.com/your-repo/laptop-price-prediction.git
   ```
2. Navigate to the project directory.
   ```sh
   cd laptop-price-prediction
   ```
3. Install the required packages.
   ```sh
   pip install -r requirements.txt
   ```

## Usage

1. Run the data scraping script from the linked repository.
2. Perform data cleaning and analysis as described.
3. Execute the EDA scripts.
4. Train the model using the provided pipeline code.
5. Evaluate the model using the evaluation script.
6. Create a pickle file of the model.
7. Launch the Streamlit app.
   ```sh
   streamlit run app.py
   ```
