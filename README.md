
# 🏙 New York Airbnb EDA Project

This project performs **Exploratory Data Analysis (EDA)** on a dataset of Airbnb listings in New York City.
The analysis includes **data cleaning, visualization, and feature engineering** to uncover patterns in pricing, availability, and listing attributes across different boroughs and room types.

---

## 📂 Project Overview

The primary goals of this project are:

* Load and explore the Airbnb dataset.
* Clean and preprocess the data by handling missing values, duplicates, and data types.
* Analyze the distribution of key features such as price, availability, and reviews.
* Explore relationships between variables using univariate, bivariate, and geographical visualizations.
* Engineer new features for deeper insights.

---

## 📊 Dataset

**Source:** `airbnb_dataset.csv` (sample data from Airbnb NYC listings)
**Size:** 20,724 rows × 22 columns

**Key Columns:**

* `neighbourhood_group` – NYC boroughs (Manhattan, Brooklyn, Queens, Bronx, Staten Island)
* `room_type` – Type of listing (Entire home/apartment, Private room, etc.)
* `price` – Listing price per night (USD)
* `minimum_nights` – Minimum stay requirement
* `number_of_reviews` – Number of guest reviews
* `availability_365` – Availability throughout the year
* `latitude` & `longitude` – Geographical coordinates

---

## 🔧 Steps & Methods

### 1. **Importing Dependencies**

Libraries used:

```python
pandas, numpy, matplotlib, seaborn
```

### 2. **Data Cleaning**

* Removed rows with null values.
* Dropped duplicate entries.
* Converted columns to correct data types.
* Removed extreme outliers (prices above \$1500).

### 3. **Exploratory Data Analysis (EDA)**

**Univariate Analysis**

* Distribution plots for `price` and `availability_365`.
* Average price per neighbourhood group.

**Feature Engineering**

* Added `price_per_bed` column to normalize price by number of beds.

**Bivariate Analysis**

* Price comparison across neighbourhood groups and room types.
* Relationship between price and number of reviews.
* Pairplots of numerical features segmented by room type.

**Geospatial Analysis**

* Scatterplot of listings based on latitude & longitude with room type color coding.

---

## 📈 Key Insights

* **Manhattan** has the highest average listing prices, followed by Brooklyn.
* **Price per bed** is significantly higher in Manhattan than other boroughs.
* Most listings are concentrated in Manhattan and Brooklyn.
* Entire home/apartment listings are more expensive compared to shared or private rooms.

---

## 📷 Visualizations

The project includes:

* **Boxplots & Histograms** – Price distribution & availability patterns.
* **Barplots** – Average price per neighbourhood and room type.
* **Scatterplots** – Price vs. reviews & geographical mapping.
* **Pairplots** – Multi-variable relationships.

---

## 🚀 How to Run

1. Clone this repository:

```bash
git clone https://github.com/yourusername/NewYorkAirbnbEDA.git
cd NewYorkAirbnbEDA
```

2. Install dependencies:

```bash
pip install pandas numpy matplotlib seaborn
```

3. Run the Jupyter Notebook or Google Colab file:

```bash
jupyter notebook New_York_Airbnb_EDA_Project.ipynb
```

---

## 📌 Requirements

* Python 3.7+
* Pandas, NumPy, Matplotlib, Seaborn
* Jupyter Notebook / Google Colab

I can also make you a **short, recruiter-friendly GitHub description** for this project so it looks professional when someone visits your repo.
Do you want me to prepare that next?
