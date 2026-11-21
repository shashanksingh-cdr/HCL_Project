# Phone Sales Data Analysis Project

## 1. Project Overview

This project focuses on analysing phone sales data using Python to understand sales performance, customer behaviour, and business trends.

The main objective is to clean and analyse the dataset, identify important sales patterns, and provide meaningful insights and recommendations to help the sales manager make better business decisions.

## 2. Project Objectives

- Clean and preprocess raw phone sales data.
- Identify and handle missing values and duplicate records.
- Perform exploratory data analysis (EDA).
- Analyse sales performance across different cities, phone segments, and sales channels.
- Study the relationship between discounts, customer footfall, customer ratings, advertising expenditure, and units sold.
- Identify low-performing sales records.
- Provide business insights and recommendations.

## 3. Tools and Technologies Used

| Tool / Library | Purpose |
|---|---|
| Python | Programming language |
| Pandas | Data cleaning and manipulation |
| NumPy | Numerical operations |
| Matplotlib | Data visualisation |
| Seaborn | Statistical graphs and visualisation |
| Jupyter Notebook | Writing and executing Python code |
| VS Code | Development environment |
| Git | Version control |
| GitHub | Project hosting and documentation |

## 4. Dataset Description

The project uses a phone sales dataset containing information about weekly phone sales.

**Original Dataset:**
- Total Records: 255
- Total Columns: 11

**Important Columns:**

| Column | Description |
|---|---|
| Record_ID | Unique identification number |
| Week_Start_Date | Starting date of the sales week |
| City | City where sales were recorded |
| Phone_Segment | Budget, Mid-Range, or Premium |
| Sales_Channel | Distributor, Online, or Retail Store |
| Avg_Price_INR | Average phone price in INR |
| Discount_Percent | Discount percentage offered |
| Ad_Spend_INR | Advertising expenditure in INR |
| Weekly_Footfall | Number of customers visiting |
| Customer_Rating | Customer rating |
| Units_Sold | Number of phones sold |

## 5. Data Cleaning and Preprocessing

The original dataset was examined and cleaned to improve data quality.

The following operations were performed:

- Removed duplicate records.
- Handled missing values.
- Standardised inconsistent categorical text.
- Checked and handled invalid values.
- Corrected data types where required.
- Checked for duplicate IDs.

**Final Dataset:**
- Total Records: 250
- Total Columns: 11
- Missing Values: 0
- Duplicate Rows: 0
- Duplicate IDs: 0

## 6. Feature Engineering

Two additional columns were created to support further analysis:

**1. Estimated_Revenue_INR**

Calculated by multiplying Units Sold by Average Price.

`Estimated Revenue = Units Sold × Average Price`

This represents estimated revenue before discounts.

**2. Sales_Status**

Classified sales records into two categories:
- At Risk: Units Sold below 25.
- Normal: Units Sold equal to or above 25.

**3. Footfall_Band**

Divided weekly customer footfall into three categories:
- Low
- Medium
- High

The enhanced dataset contains 250 records and 14 columns.

## 7. Exploratory Data Analysis (EDA)

The following analyses were performed:

- Overall distribution of units sold.
- Sales performance by city.
- Sales performance by phone segment.
- Sales performance by sales channel.
- Relationship between discounts and units sold.
- Relationship between customer footfall and units sold.
- Correlation analysis of numerical variables.
- Identification of at-risk sales records.

## 8. Key Insights

### City-wise Sales Performance

| City | Average Units Sold |
|---|---:|
| Jaipur | 44.40 |
| Pune | 41.26 |
| Delhi | 41.26 |
| Lucknow | 39.58 |
| Mumbai | 38.84 |

Jaipur recorded the highest average sales, while Mumbai recorded the lowest.

### Phone Segment Performance

| Phone Segment | Average Units Sold |
|---|---:|
| Budget | 41.48 |
| Mid-Range | 40.29 |
| Premium | 38.48 |

Budget phones recorded the highest average sales.

### Sales Channel Performance

| Sales Channel | Average Units Sold |
|---|---:|
| Distributor | 40.86 |
| Online | 40.82 |
| Retail Store | 40.29 |

All three sales channels showed relatively similar performance.

### Correlation Analysis

| Factor | Correlation with Units Sold |
|---|---:|
| Weekly Footfall | +0.614 |
| Discount Percentage | +0.497 |
| Customer Rating | +0.007 |
| Advertising Spend | -0.111 |

Weekly Footfall showed the strongest positive correlation with Units Sold, followed by Discount Percentage.

Correlation indicates association and does not establish causation.

### At-Risk Sales Analysis

Out of 250 sales records:
- Normal: 216 records (86.4%)
- At Risk: 34 records (13.6%)

City-wise distribution of at-risk records:

| City | At-Risk Records |
|---|---:|
| Mumbai | 11 |
| Delhi | 10 |
| Lucknow | 7 |
| Pune | 6 |
| Jaipur | 0 |

Mumbai and Delhi had the highest numbers of at-risk records.

## 9. Business Recommendations

1. Improve sales performance in Mumbai and Delhi by investigating the reasons for low-performing records.
2. Maintain adequate stock of budget phones because they have the highest average sales.
3. Introduce targeted promotional strategies to improve premium phone sales.
4. Focus on increasing customer footfall through local marketing and promotional activities.
5. Use discounts strategically and monitor their impact on sales.
6. Evaluate advertising campaigns before increasing advertising expenditure.
7. Monitor at-risk sales records and take corrective action.

## 10. Project Folder Structure

```text
Phone-Sales-Data-Analysis/
│
├── data/
│   ├── raw/
│   │   └── phone_sales_data.csv
│   │
│   └── processed/
│       ├── phone_sales_cleaned.csv
│       └── phone_sales_cleaned_added_columns.csv
│
├── notebooks/
│   └── phone_sales_analysis.ipynb
│
├── images/
│
├── scripts/
│
└── README.md
```

## 11. How to Run the Project

1. Clone or download this repository.
2. Open the project folder in VS Code.
3. Install the required Python libraries:

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

4. Open the Jupyter Notebook:

```text
notebooks/phone_sales_analysis.ipynb
```

5. Run the notebook cells to perform data cleaning, feature engineering, exploratory data analysis, and visualisation.

Make sure the dataset files are available in the specified folders.

## 12. Conclusion

This project demonstrates how Python can be used for data cleaning, feature engineering, exploratory data analysis, and business decision-making.

The analysis identified differences in city-wise sales performance, phone segment preferences, and the relationship between customer footfall, discounts, and units sold.

The insights and recommendations can help a sales manager identify areas requiring improvement and make more informed business decisions.

---

**Project Category:** Data Analytics

**Programming Language:** Python

**Status:** Completed
