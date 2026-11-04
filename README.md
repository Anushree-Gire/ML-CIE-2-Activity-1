# ML CIE 2 – Activity 1: Dataset Preparation and EDA

## Project Overview
This project focuses on dataset preparation and Exploratory Data Analysis (EDA) using the Hotel Booking Demand dataset.

The objective is to understand and perform essential data preprocessing techniques before applying machine learning algorithms.

## Dataset Information
- **Dataset:** Hotel Booking Demand
- **Source:** [Kaggle – Hotel Booking Demand Dataset](https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand)
- **Original Dataset:** `hotel_bookings.csv`

The dataset contains hotel booking information, including booking dates, guest details, stay duration, booking channels, room types, and cancellation status.

## Technologies and Libraries Used
- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## Activities Performed
1. Dataset loading and inspection
2. Identification of numerical and categorical features
3. Handling missing values
4. Duplicate record removal
5. Categorical data inspection
6. Exploratory Data Analysis (EDA)
7. Data visualization using histograms, count plots, and box plots
8. Categorical encoding using numerical mapping and One-Hot Encoding
9. Numerical feature scaling using StandardScaler
10. Final dataset verification and export

## Final Dataset
- **Rows:** 86,871
- **Columns:** 72
- **Missing Values:** 0
- **Duplicate Records:** 0

The final prepared dataset is available as `hotel_bookings_prepared.csv.gz`.

To extract it, use:

```python
import gzip
import shutil

with gzip.open('hotel_bookings_prepared.csv.gz', 'rb') as source:
    with open('hotel_bookings_prepared.csv', 'wb') as target:
        shutil.copyfileobj(source, target)
```

## Project Files
- `Ml_activity_1 (1).ipynb` – Completed Jupyter Notebook
- `hotel_bookings.csv` – Original dataset
- `hotel_bookings_prepared.csv.gz` – Final prepared dataset

## Conclusion
The activity demonstrates the importance of data cleaning, exploratory data analysis, encoding, and feature scaling in preparing real-world datasets for machine learning applications.
