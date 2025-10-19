# Hotel_Project
#  Hotel Booking Analysis and Cancellation Prediction using Python

This project analyzes and predicts hotel booking cancellations using **Python**, combining data from multiple years of bookings.  
It includes **data cleaning**, **feature engineering**, **EDA**, and **machine learning models** to uncover key business insights and improve hotel performance.

---

##  Project Objectives
- Combine multiple hotel booking datasets into a unified analytical dataset.  
- Perform **Exploratory Data Analysis (EDA)** to uncover customer behavior and seasonal trends.  
- Engineer new features (e.g., `total_stays`, `total_guests`, `booking_source`, `total_booking_revenue`).  
- Predict **booking cancellations** using different machine learning models.  
- Visualize insights about revenue, customer segmentation, and booking behavior.

---

##  Tools & Libraries
- **Python**  
- **Pandas**, **NumPy**, **Matplotlib**, **Seaborn**  
- **Scikit-learn** (Decision Tree, Random Forest, Logistic Regression)  
- **Data Visualization** for EDA and insights presentation  

---

##  Key Analysis Steps
1. **Data Integration & Cleaning**
   - Merged multiple CSV files into one dataset.  
   - Handled missing data (`children`, `country`, `agent`, `company`).  
   - Fixed inconsistent country codes and undefined categories.

2. **Feature Engineering**
   - Created derived fields like:
     - `total_stays`, `total_guests`, `is_family`
     - `total_meal_revenue`, `discount_value`, `net_revenue_after_discount`
     - `booking_source`, `total_booking_revenue`
   - Capped extreme outliers and removed unrealistic values.

3. **Exploratory Data Analysis (EDA)**
   - Correlation heatmap to identify strong relationships.  
   - Insights on:
     - Cancellation rate by month, hotel, and distribution channel.  
     - Impact of lead time, ADR, and total stays on cancellations.  
     - Revenue analysis by year, month, country, and room type.  

4. **Machine Learning Models**
   - **Decision Tree Classifier** → Overfitted (Train=100%, Test=87%)  
   - **Random Forest Classifier** → Best performance (Train=100%, Test=99%)  
   - **Logistic Regression** → Stable baseline (Train=83%, Test=84%)

---

##  Business Insights
- Higher **lead time** and **fewer special requests** increase cancellation likelihood.  
- **Family bookings** tend to stay longer and generate higher revenue.  
- **Online TA/TO** is the dominant booking channel.  
- **Random Forest** was the most accurate model for predicting cancellations.

---

##  Results Summary
| Model | Train Accuracy | Test Accuracy | Precision | Recall | Notes |
|-------|----------------|---------------|------------|---------|--------|
| Decision Tree | 100% | 87% | 0.82 | 0.83 | Overfitting |
| Random Forest | 100% | **99%** | 1.00 | 0.98 | Best model |
| Logistic Regression | 83% | 84% | 0.80 | 0.75 | Baseline model |

---

##  Visualization Examples
- Cancellation rates by month, hotel, and channel.  
- Revenue trends by year and country.  
- Relationship between ADR, discount, and total revenue.  
- Booking patterns by family size and customer type.


