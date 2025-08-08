
#  New York Airbnb EDA Project

This project focuses on **Exploratory Data Analysis (EDA)** of New York City Airbnb listings.
It covers data loading, cleaning, visualization, and feature engineering to identify trends and patterns in pricing, availability, and other attributes.

---

## 📂 Project Overview

The aim of this project is to:

* Load and explore the Airbnb dataset.
* Clean and preprocess data by handling missing values, duplicates, and incorrect data types.
* Perform statistical analysis and create visualizations.
* Derive insights about pricing, availability, reviews, and location-based trends.

---

## 📊 Dataset

* **File Name:** `airbnb_dataset.csv`
* **Entries:** 20,724 rows × 22 columns
* **Key Columns:**

  * `neighbourhood_group` – Borough in NYC (Manhattan, Brooklyn, Queens, Bronx, Staten Island)
  * `room_type` – Type of listing (Entire home/apartment, Private room, etc.)
  * `price` – Price per night in USD
  * `minimum_nights` – Minimum nights required to book
  * `number_of_reviews` – Number of guest reviews received
  * `reviews_per_month` – Average reviews per month
  * `availability_365` – Availability days in a year
  * `latitude`, `longitude` – Geographic coordinates

---

## 🔧 Steps in the Project

### 1. Importing Dependencies

* Libraries used: `pandas`, `numpy`, `matplotlib`, `seaborn`

### 2. Data Cleaning

* Removed rows with missing values.
* Dropped duplicate records.
* Converted data types for appropriate columns.
* Removed price outliers (listings priced above \$1500).

### 3. Exploratory Data Analysis

**Univariate Analysis**

* Distribution of `price` and `availability_365`
* Average price per neighbourhood group

**Feature Engineering**

* Created `price_per_bed` column to better compare listings with different bed counts

**Bivariate Analysis**

* Barplots comparing prices across neighbourhoods and room types
* Scatterplots of price vs number of reviews
* Pairplots of numerical features segmented by room type

**Geospatial Analysis**

* Scatterplot mapping listings using latitude & longitude

**Correlation Analysis**

* Heatmap to identify relationships between numerical variables

---

## 📈 Key Insights

* Manhattan has the highest average listing prices, followed by Brooklyn.
* Price per bed is significantly higher in Manhattan than other boroughs.
* Most listings are concentrated in Manhattan and Brooklyn.
* Entire home/apartment listings are more expensive compared to shared or private rooms.
* Number of reviews and reviews per month have a **strong positive correlation (0.63)** — listings with more total reviews tend to receive them more frequently.
* Price and beds show a **moderate correlation (0.42)** — listings with more beds tend to be priced higher.
* Longitude and price have a **weak negative correlation (-0.19)** — slight east–west effects on pricing.
* Most other numerical features show **very low correlations**, indicating minimal linear relationships.

---

## 📷 Visualizations Included

* Boxplots and histograms of price and availability distributions
* Barplots of prices by neighbourhood and room type
* Scatterplots of price vs number of reviews and geospatial location mapping
* Pairplots of multiple features segmented by room type
* Correlation heatmap of numerical features
