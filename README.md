#  Bangalore House Price Analysis

##  Project Overview

This project focuses on analyzing housing prices in Bangalore using the **house_price.csv** dataset. The goal is to perform exploratory data analysis (EDA), detect and handle outliers, and understand relationships between variables such as price, area, and number of rooms.

---

##  Dataset Description

The dataset contains information about residential properties in Bangalore.

###  Key Features:

* **location** – Area where the property is located
* **size** – Number of bedrooms (BHK)
* **total_sqft** – Total area of the property (in square feet)
* **bath** – Number of bathrooms
* **price** – Price of the property (in lakhs)

###  Engineered Feature:

* **price_per_sqft** – Calculated as:
  `price_per_sqft = (price × 100000) / total_sqft`

---

##  Objectives

* Perform **Exploratory Data Analysis (EDA)**
* Detect and remove **outliers** using multiple statistical techniques
* Analyze data distribution and apply **transformations**
* Study relationships between variables using **correlation and plots**

---

##  Exploratory Data Analysis (EDA)

* Checked dataset structure using `.info()` and `.describe()`
* Identified missing values and handled them
* Created new feature: `price_per_sqft`
* Visualized distributions using histograms and boxplots

---

##  Outlier Detection Methods

Outliers were detected and removed using:

1. **Mean & Standard Deviation Method**
2. **Percentile Method (1%–99%)**
3. **Interquartile Range (IQR) Method**
4. **Z-Score Method**

 Among these, the **IQR method** was found to be the most effective for this dataset.

---

##  Data Visualization

* **Box Plots** – Used to identify and compare outliers
* **Histogram (Histplot)** – Checked distribution of `price_per_sqft`
* **Scatter Plots** – Analyzed relationships between variables
* **Heatmap** – Visualized correlation between numerical features

---

##  Data Transformation

* Observed that `price_per_sqft` was **right-skewed**
* Applied **log transformation** to normalize the data
* Compared **skewness and kurtosis** before and after transformation

---

##  Correlation Analysis

* Strong positive correlation found between:

  * `price` and `total_sqft`
* Moderate correlation with:

  * `bath` and `size`

---

##  Data Cleaning Steps

* Removed duplicate records
* Handled missing values
* Removed outliers using statistical methods
* Reset index after cleaning

---

##  Conclusion

* The dataset initially contained significant outliers and skewness
* IQR method effectively removed extreme values
* Log transformation improved data normality
* Property price is strongly influenced by total square footage

---

##  Tools & Libraries Used

* Python 
* Pandas
* NumPy
* Matplotlib
* Seaborn
* SciPy

---

##  How to Run the Project

1. Load the dataset:

   ```python
   df = pd.read_csv("house_price.csv")
   ```
2. Perform EDA and preprocessing
3. Apply outlier detection methods
4. Visualize data using plots

---


---

## 👨‍💻 Author

Sreehari

---
