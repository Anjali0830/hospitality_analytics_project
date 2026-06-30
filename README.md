# Hospitality Analytics Project
## Customer Retention and Dynamic Pricing Analysis in the Hospitality Industry

![Python](https://img.shields.io/badge/Python-3.10-blue)
![Power BI](https://img.shields.io/badge/PowerBI-Dashboard-yellow)
![Machine Learning](https://img.shields.io/badge/MachineLearning-LogisticRegression-green)
![Status](https://img.shields.io/badge/Project-Completed-success)

---

## Project Overview

The hospitality industry faces significant challenges related to booking cancellations, customer retention, revenue optimization, and dynamic pricing.

This project analyzes hotel booking data to identify customer behavior patterns, evaluate cancellation trends, optimize pricing strategies, and build a machine learning model to predict booking cancellations.

The project combines:

- Data Cleaning & Preprocessing
- Exploratory Data Analysis (EDA)
- Customer Segmentation
- Cancellation Prediction
- Dynamic Pricing Analysis
- Power BI Dashboard Development

---

## Business Problem

Hotel businesses frequently experience:

- High booking cancellation rates
- Revenue loss due to cancellations
- Seasonal demand fluctuations
- Inefficient pricing strategies
- Customer retention challenges

The objective of this project is to generate actionable insights that help hotels improve customer retention and maximize revenue.

---

## Dataset Information

### Dataset

Hotel Booking Demand Dataset

### Features Available

```text
hotel
is_canceled
lead_time
arrival_date_year
arrival_date_month
arrival_date_week_number
arrival_date_day_of_month
stays_in_weekend_nights
stays_in_week_nights
adults
children
babies
meal
country
market_segment
distribution_channel
is_repeated_guest
previous_cancellations
previous_bookings_not_canceled
reserved_room_type
assigned_room_type
booking_changes
deposit_type
agent
company
days_in_waiting_list
customer_type
adr
required_car_parking_spaces
total_of_special_requests
reservation_status
reservation_status_date
```

### Removed Sensitive Columns

```text
name
email
phone-number
credit_card
```

---

## Project Objectives

- Perform data cleaning and preprocessing.
- Analyze hotel booking trends.
- Identify major cancellation factors.
- Analyze customer segments.
- Develop a cancellation prediction model.
- Build an interactive Power BI dashboard.
- Generate business recommendations.


# Data Cleaning & Preprocessing

The following preprocessing steps were performed:

### Missing Value Handling

Missing values were handled for:

- children
- country
- agent
- company

### Duplicate Removal

Duplicate hotel booking records were identified and removed.

### Feature Engineering

New features created:

### Total Guests

```python
total_guests = adults + children + babies
```

### Total Stay

```python
total_stay = stays_in_weekend_nights + stays_in_week_nights
```

### Total Revenue

```python
total_revenue = adr * total_stay
```

---

# Exploratory Data Analysis

The following analyses were performed:

### Cancellation Analysis

- Cancellation Distribution
- Lead Time vs Cancellation
- ADR vs Cancellation

### Customer Analysis

- Customer Type Distribution
- Repeat Guest Analysis
- Country Analysis

### Booking Analysis

- Monthly Booking Trends
- Hotel Type Distribution
- Market Segment Analysis

### Pricing Analysis

- ADR by Month
- ADR by Market Segment
- Revenue Trends

---

# Machine Learning Model

## Objective

Predict whether a booking will be canceled.

### Target Variable

```text
is_canceled
```

### Features Used

```text
lead_time
adr
adults
children
total_stay
previous_cancellations
booking_changes
```

### Algorithm

```text
Logistic Regression
```

### Train-Test Split

```text
Training Data: 80%
Testing Data: 20%
```

---

## Model Performance

### Classification Report

| Metric | Score |
|----------|----------|
| Accuracy | 73% |
| Weighted Precision | 69% |
| Weighted Recall | 73% |
| Weighted F1 Score | 66% |

### Interpretation

The model achieved an overall accuracy of 73%.

The model performed well in identifying non-cancelled bookings but struggled to identify cancelled bookings due to class imbalance.

Future improvements may include:

- Random Forest
- XGBoost
- SMOTE
- Hyperparameter Tuning

---

# Power BI Dashboard

The project includes an interactive Power BI dashboard consisting of four pages.

## Page 1: Executive Overview

KPIs:

- Total Bookings
- Total Revenue
- Average ADR
- Cancellation Rate

Visualizations:

- Monthly Booking Trend
- Hotel Type Distribution

---

## Page 2: Cancellation Analysis

Visualizations:

- Cancellation by Market Segment
- Cancellation by Country
- Lead Time vs Cancellation
- Customer Type Analysis

---

## Page 3: Dynamic Pricing Analysis

Visualizations:

- ADR by Month
- ADR by Market Segment
- Revenue by Hotel Type
- ADR vs Total Guests

---

## Page 4: Customer Segmentation

Visualizations:

- Customer Type Distribution
- Repeat Guest Analysis
- Country Analysis
- Market Segment Distribution

---

# Key Findings

### Customer Cancellation

- Longer lead times significantly increase cancellation probability.
- Some market segments contribute disproportionately to cancellations.

### Customer Retention

- Repeat guests demonstrate stronger retention behavior.
- Loyal customers generate more stable revenue streams.

### Dynamic Pricing

- ADR varies significantly across seasons.
- Pricing patterns differ across customer segments.

### Revenue

- Seasonal demand strongly impacts revenue generation.
- Revenue optimization opportunities exist during peak demand periods.

---

# Business Recommendations

### Reduce Cancellations

- Introduce predictive cancellation monitoring.
- Offer flexible rebooking options.
- Provide early confirmation incentives.

### Improve Revenue

- Implement dynamic pricing strategies.
- Increase ADR during peak demand periods.

### Improve Customer Retention

- Develop loyalty programs.
- Offer personalized promotions.
- Reward repeat guests.

---

# Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- Power BI
- GitHub

---

# Future Enhancements

Potential improvements include:

- Random Forest Classifier
- XGBoost Model
- Real-Time Booking Predictions
- Customer Lifetime Value Analysis
- Demand Forecasting
- Automated Pricing Recommendations

---

# Author

**Anjali Gurav**

Hospitality Analytics Project

Data Analytics Internship Project

---

# License

This project is intended for educational and portfolio purposes.





---
