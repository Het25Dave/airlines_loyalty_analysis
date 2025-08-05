# 1. Customer Loyalty EDA Report 

This document serves as an analysis summary of your customer loyalty dataset and the main findings from your EDA.

## Project Overview

This project explores customer characteristics, loyalty program adoption, and behavioral metrics in a Canadian customer base. The exploratory analysis focuses on demographic features, enrollment and cancellation activity, loyalty card types, and how these factors interact with Customer Lifetime Value (CLV).

## Data Structure

Key columns include:

- loyalty_number, country, province, city, postal_code
- gender, education, salary, maratial_status
- loyalty_card (Aurora, Nova, Star)
- clv (Customer Lifetime Value)
- enrollment_type (Standard, 2018 Promotion), enrollment_year, enrollment_month
- cancellation_year, cancellation_month
- enrollment_date, cancellation_date

The data is primarily from Canadian cities, with salary and cancellation data occasionally missing.

## Summary of Main Insights

### A. City and Loyalty Card Distribution

- Toronto, Vancouver, and Montreal are the top cities for customer count in all card types.
- Loyalty cards are distributed mainly among Aurora, Nova, and Star, with "Star" being the most common.

| City | Aurora | Nova | Star | Total |
| :-- | :-- | :-- | :-- | :-- |
| Toronto | 719 | 1123 | 1509 | 3351 |
| Vancouver | 526 | 869 | 1187 | 2582 |
| Montreal | 412 | 693 | 954 | 2059 |

### B. Enrollment and Promotion

- Most enrollments are "Standard."
- The "2018 Promotion" led to sharp enrollment increases in 2018, but the base remains overwhelmingly "Standard."


### C. Loyalty Card and CLV

- Aurora members are the highest average CLV holders (10,672.69), followed by Nova (8,045.62) and Star (6,741.76).
- Median CLV mirrors this relationship.


### D. Marital Status and CLV

- Divorced and Married have higher mean CLVs (8,200.69 and 8,058.20) compared to Singles (7,719.49).
- Divorced show the highest median CLV (5,872.96).


### E. Enrollment \& Cancellation Trends

- Enrollments peak in 2018 due to promotions.
- Cancellations have steadily risen over time for all marital statuses.


## Conclusions \& Recommendations

- Target growth efforts in Toronto, Vancouver, and Montreal.
- Consider Aurora upgrades for high-CLV candidates.
- Review why cancellations are rising, especially among married and high-value customers.
- Address missing salary information for improved modeling.
- Explore advanced segmentations (education, gender) in further analysis.


# 2. Plot Explanations Report (Text File)

This document explains the plots and tables generated in the EDA notebook:

## 1. Loyalty Card Distribution by City

**Plot/Table:** Shows count of customers per city split by loyalty card (Aurora, Nova, Star).
**Interpretation:** Toronto, Vancouver, and Montreal are the dominant cities for all card types. Aurora customers are somewhat less common, but Star dominates overall.

## 2. Enrollment Type by City

**Plot/Table:** Customer count by city, split between "2018 Promotion" and "Standard" enrollment types.
**Interpretation:** The bulk of enrollments are "Standard," with a visible (but much smaller) spike for "2018 Promotion" in 2018.

## 3. Loyalty Card CLV Analysis

**Plot/Table:** Aggregated CLV for each loyalty card type, showing total, average, and median CLV.
**Interpretation:** Aurora customers provide the highest lifetime value on average; promotional intervention might focus on migrating more users to this tier.

## 4. CLV by Marital Status

**Plot/Table:** Mean, median, and count of CLV per marital status.
**Interpretation:** Divorced and married customers are more valuable on average than singles, and this trend holds for the median.

## 5. Enrollment Trends by Year and Marital Status

**Plot/Table:** Yearly enrollment counts for Divorced, Married, and Single.
**Interpretation:** Enrollment grew yearly, peaking in 2018.

## 6. Cancellation Trends by Year and Marital Status

**Plot/Table:** Yearly cancellation counts for Divorced, Married, and Single.
**Interpretation:** Cancellations increase yearly for all groups, with most among married users.
