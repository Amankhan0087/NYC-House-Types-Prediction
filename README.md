# NYC House Types Prediction

Exploratory data analysis and machine learning project that studies Airbnb listings in New York City and works toward predicting the listing/room type from listing attributes.

## Overview

This project analyzes the New York City Airbnb Open Data dataset to understand pricing, availability, and neighbourhood patterns, with the goal of building a model that predicts the room type of a listing (e.g. Entire home/apt, Private room, Shared room) from its other features.

## Dataset

- Source: Kaggle - New York City Airbnb Open Data
- Kaggle handle: dgomonov/new-york-city-airbnb-open-data
- File used: AB_NYC_2019.csv
- Size: 48,895 listings across 16 columns
- Key columns: id, name, host_id, host_name, neighbourhood_group, neighbourhood, latitude, longitude, room_type, price, minimum_nights, number_of_reviews, last_review, reviews_per_month, calculated_host_listings_count, availability_365

## Project Structure

- NYC_House_Types_Prediction_.ipynb - main Jupyter/Colab notebook containing the full analysis

## Tech Stack
- Python 3
- pandas and numpy for data manipulation
- matplotlib and seaborn for visualization
- scikit-learn for train/test splitting and modeling
- kagglehub for dataset download
- Google Colab / Jupyter Notebook

## Getting Started

### Prerequisites

```bash
pip install numpy pandas matplotlib seaborn scikit-learn kagglehub
```

### Running the Notebook

1. Open NYC_House_Types_Prediction_.ipynb in Google Colab or Jupyter
2. Run the cells in order to download the dataset and reproduce the analysis

## Current Progress

- Dataset loading via kagglehub
- Initial data exploration (head, info, describe, shape)
- Missing value inspection
- Exploratory visualizations: room type distribution, neighbourhood group distribution, numeric feature histograms, price vs. room type (boxen plot), feature correlation heatmap, and latitude/longitude scatterplot
- Data cleaning: dropped non-predictive columns (id, name, host_id, host_name, last_review), filled missing reviews_per_month values with 0, and capped extreme outliers in price and minimum_nights at the 99th percentile
- Train/test split (67/33) prepared for modeling using scikit-learn

## Roadmap

- Train and evaluate a room type classification model
- Model evaluation and performance tuning

## Author

Maintained by Amankhan0087.
