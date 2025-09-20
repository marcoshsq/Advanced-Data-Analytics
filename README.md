# 🚖 Automatidata Project – Course 2 (Google Advanced Data Analytics)

## 📌 Overview

This repository contains my solution to the **Course 2 End-of-Course Project** from the [Google Advanced Data Analytics Certificate](https://www.coursera.org/professional-certificates/google-advanced-data-analytics).
The project simulates a workplace scenario at **Automatidata**, a fictional data consulting firm, which is collaborating with the **New York City Taxi and Limousine Commission (TLC)**.

The main goal of this project was to **inspect, clean, and organize the NYC Yellow Taxi dataset** to ensure it is ready for exploratory data analysis (EDA), visualizations, and predictive modeling.

---

## 🗂 Dataset

* **Name:** 2017 Yellow Taxi Trip Data
* **Rows:** \~408,000
* **Columns:** 18
* **Source:** Provided for educational purposes (pedagogical dataset, not official TLC data)

Key columns include:

* `trip_distance` – distance traveled (miles)
* `fare_amount` – fare based on time and distance
* `total_amount` – total charge to passenger
* `tpep_pickup_datetime` / `tpep_dropoff_datetime` – trip timestamps
* `Passenger_count`, `RateCodeID`, `Payment_type`, `VendorID`
* Various surcharges, tips, and tolls

---

## 🛠️ Project Tasks

This project follows the **PACE framework** (Plan, Analyze, Construct, Execute).

### ✔️ Plan

* Review dataset and project documentation
* Identify relevant vs. irrelevant variables
* Define goals: ensure data readiness for modeling

### ✔️ Analyze

* Build dataframe with **pandas**
* Run `.info()`, `.describe()`, and missing value checks
* Detect anomalies (e.g., negative fares, extreme distances)

### ✔️ Execute

* Create **derived variables**:

  * Trip duration (minutes)
  * Fare per mile
  * Temporal features (hour, weekday, rush hour)
* Summarize dtypes, null counts, and unique values
* Generate descriptive statistics for key KPIs

---

## 📊 Key Findings

* Dataset contains outliers: unusually long trips (>100 miles) and negative/zero fares.
* **Trip distance** and **pickup datetime** (plus derived features) are the two most useful variables for building a predictive fare model.
* Additional relevant features: `RateCodeID`, `Payment_type`, `PULocationID`, `DOLocationID`.
* Some columns (e.g., `store_and_fwd_flag`, `ID`) are less relevant for modeling.

---

## 📈 Next Steps

* Handle outliers and missing values (cleaning).
* Explore integration of external data (weather, holidays, events).
* Prepare dataset for regression modeling (Course 3+).
* Build predictive model for taxi fares.

---

## ⚙️ Tools & Libraries

* Python 3
* pandas, numpy
* Jupyter Notebook

---

## 👤 Author

**Marcos Henrique Silva Quirino**

* [LinkedIn](https://www.linkedin.com/in/marcoshsq/)
* [GitHub](https://github.com/marcoshsq)

---

✨ *This project is part of my learning journey in Data Analytics & Business Intelligence. Feedback and suggestions are welcome!*

---
