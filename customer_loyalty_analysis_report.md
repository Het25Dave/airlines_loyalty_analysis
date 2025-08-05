# Project Report: Exploratory Data Analysis (EDA) for Customer Loyalty

## 1. Introduction

This report presents the Exploratory Data Analysis (EDA) conducted on a customer loyalty dataset. The primary aim is to understand the demographic and behavioral features of customers, distribution and performance of different loyalty cards, enrollment and cancellation trends, and factors impacting Customer Lifetime Value (CLV).

## 2. Data Overview

**Dataset columns include:**

- Loyalty Number
- Country, Province, City, Postal Code
- Gender, Education, Salary, Marital Status
- Loyalty Card Type
- Customer Lifetime Value (CLV)
- Enrollment Type, Year, Month
- Cancellation Year, Month

**Sample Data Insights:**

- All customers are from Canada, covering various provinces and cities.
- Key categorical variables: gender, education, marital status, loyalty card, enrollment and cancellation data.
- Salary and CLV are numerical.
- Some missing data observed (e.g., incomplete salary, missing cancellation dates).


## 3. Data Cleaning \& Preparation

**Actions Taken:**

- Imported essential Python libraries: pandas, numpy, matplotlib, seaborn.
- Loaded and visualized data samples.

**Data Adjustments:**

- Standardized missing values (e.g., NaN for missing salary/cancellation info).
- Added or reformatted features such as combined date fields (e.g., `enrollment_date`, `cancellation_date`).


## 4. Exploratory Data Analysis

### a. Distribution of Loyalty Cards by City

**Findings:**

- The top cities with loyalty card holders are Toronto, Vancouver, and Montreal.
- Each city has customers distributed across three main loyalty card types: Aurora, Nova, and Star.
- Toronto holds the highest customer count across all card types.

**Data Table Example (Top Cities):**


| City | Aurora | Nova | Star | Total |
| :-- | :-- | :-- | :-- | :-- |
| Toronto | 719 | 1123 | 1509 | 3351 |
| Vancouver | 526 | 869 | 1187 | 2582 |
| Montreal | 412 | 693 | 954 | 2059 |

### b. Enrollment Type Breakdown

**Findings:**

- There are two enrollment types: Standard and 2018 Promotion.
- Most enrollments happened under the 'Standard' type.
- For instance, in Toronto, only 173 out of 3351 enrollments were from the promotion.

| City | 2018 Promotion | Standard | Total |
| :-- | :-- | :-- | :-- |
| Toronto | 173 | 3178 | 3351 |
| Vancouver | 151 | 2431 | 2582 |
| Montreal | 138 | 1921 | 2059 |

### c. Loyalty Card Performance (CLV Aggregation)

**Findings:**

- "Aurora" cardholders have the highest average CLV (`avg_clv`: 10,672.69), followed by "Nova" (8,045.62), and then "Star" (6,741.76).
- Median CLVs follow a similar pattern.

| Loyalty Card | Total CLV | Avg CLV | Median CLV |
| :-- | :-- | :-- | :-- |
| Aurora | 36,596,641.41 | 10,672.69 | 8140.00 |
| Nova | 45,626,688.31 | 8,045.62 | 5799.06 |
| Star | 51,486,831.60 | 6,741.76 | 4786.89 |

### d. CLV by Marital Status

**Findings:**

- Divorced and Married customers both show higher average CLV (8,200.69 and 8,058.20 respectively) than Singles (7,719.49).

| Marital Status | Mean CLV | Median CLV | Count |
| :-- | :-- | :-- | :-- |
| Divorced | 8,200.69 | 5,872.96 | 2,518 |
| Married | 8,058.20 | 5,824.77 | 9,735 |
| Single | 7,719.49 | 5,583.07 | 4,484 |

### e. Enrollment and Cancellation Trend Analysis

**Enrollment Year by Marital Status (Sample Years):**


| Year | Divorced | Married | Single |
| :-- | :-- | :-- | :-- |
| 2012 | 254 | 979 | 453 |
| 2013 | 324 | 1411 | 662 |
| 2018 | 499 | 1717 | 794 |

**Cancellation Patterns:**

- Cancellations have risen steadily from 2013 to 2018.
- Married customers have the highest cancellation count, followed by Singles and then Divorced.

| Year | Divorced | Married | Single |
| :-- | :-- | :-- | :-- |
| 2014 | 30 | 103 | 48 |
| 2015 | 31 | 172 | 62 |
| 2016 | 56 | 263 | 108 |
| 2017 | 70 | 276 | 160 |
| 2018 | 95 | 376 | 174 |

### f. Additional Insights

- **Gender, Education, Province, and Card Type correlations** can offer further insights, but are not broken out in the current output.
- **Missing salaries** are present; some customers show salary as zero or NaN, which may affect average calculations.
- **Distribution charts and plots** (not included here but generated in notebook) likely support these summary tables.


## 5. Summary \& Recommendations

- **Toronto, Vancouver, and Montreal** are the largest markets for customer loyalty programs, suggesting a focus for marketing and program development.
- **Aurora cardholders are the most valuable** on average; consider incentives to migrate high-potential customers to Aurora.
- **Married and divorced customers juggle the highest lifetime value**, but also feature prominently in cancellations, indicating possible customer lifecycle patterns worth investigating.
- **Enrollment surges in 2018** (possibly due to promotions), which could impact loyalty and retention metrics in subsequent years.
- Further analysis on features like **salary distribution, gender, and education** and their impact on CLV and cancellation are recommended.


## 6. Possible Next Steps

1. **Missing Data Handling:** Impute or analyze the impact of missing salary values.
2. **Predictive Modeling:** Use the processed data to build churn or CLV prediction models.
3. **Segmentation Analysis:** Segment the customer base for targeted marketing.
4. **Deeper Time Series Analysis:** Study how enrollment and cancellation evolve over time.

*Prepared by: Het Anand Dave*
*LinkedIn:* https://www.linkedin.com/in/hetdave200225/

