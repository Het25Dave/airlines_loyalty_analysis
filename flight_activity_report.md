Below are two detailed reports:

1. **Flight Activity Analysis Report** (main EDA findings in text format)
2. **Plot/Table Explanation Report** (explaining likely plots and tables created in the notebook)

# 1. Flight Activity Analysis Report 

## Introduction

This project analyzes flight activity for loyalty program customers. The goal is to understand flying patterns, distance and points accumulation, redemption behaviors, and top performing customers over time.

## Data Structure

Key columns include:

- loyalty_number: Unique ID for each customer.
- year, month, activity_date: Date fields.
- total_flights: Number of flights per entry.
- distance: Flight distance covered.
- points_accumulated: Points earned through flights.
- points_redeemed: Points redeemed for rewards.
- dollar_conversion_pts: Points redeemed, converted to dollars.


## Main Insights

### A. Flights, Distance, and Points (Monthly Overview)

- Each row aggregates customer activity by month.
- Most customers have multiple flights per month; a typical entry: 4 flights, 5,000–9,000 km flown, equal points accumulated, and few or no points redeemed.
- Some months have zero activity, indicating periods of inactivity for some customers.


### B. Monthly Aggregates

- Flight, distance, and redemption activity is grouped by activity_date (e.g., 2017-01).
- High-frequency flyers are visible by total_flights.
- Example: In January 2017, all customers together contributed 13,059 flights covering nearly 20 million km, with 351,520 points redeemed and about \$63,293 worth redeemed in rewards.

| activity_date | total_flights | distance | points_redeemed | dollar_conversion_pts |
| :-- | :-- | :-- | :-- | :-- |
| 2017-01 | 13,059 | 19,768,451 | 351,520 | 63,293 |

### C. Average Flight Distance per Month

- Consistent average distance per flight each month, mostly 1,480–1,515 km, indicating stable flight patterns.


### D. Top Performers

- **Top Distance Customers:** Ranked by total distance flown.
- **Top Points Redeemers:** Ranked by most points redeemed.
- **Top Frequent Flyers:** Ranked by total number of flights.


#### Sample "Top Distance Customers"

| loyalty_number | distance |
| :-- | :-- |
| 689839 | 178,858 |
| 893866 | 168,640 |
| ... | ... |

#### Sample "Top Points Redeemers"

| loyalty_number | points_redeemed |
| :-- | :-- |
| 539704 | 4,479 |
| 211755 | 4,336 |
| ... | ... |

## Conclusions \& Recommendations

- The loyalty program has clear core participants who travel frequently, fly long distances, and redeem significant points.
- Average distance per flight is broadly consistent, indicating few outliers or anomalous routes.
- Redemption rates and the dollar value of points provide insight for loyalty and marketing interventions: e.g., targeting top flyers for exclusive offers.

**Suggestions:**

- Explore inactivity periods: why do some months have zero activity for some customers?
- Segment customers by activity (distance, flights, redemption) for targeted retention strategies.
- Cross-analyze with demographic data for further insights.


# 2. Plot/Table Explanation Report 

## 1. Monthly Aggregates Plot/Table

- **Content:** Shows total flights, total distance flown, points redeemed, and dollar conversion totals for each month.
- **Purpose:** Identifies monthly seasonality or trends in loyalty activity.


## 2. Average Distance per Flight Plot/Table

- **Content:** For each month, divides total distance by total flights—visualizing consistency or changes in average journey length.
- **Purpose:** Detects shifts in flight patterns (longer or shorter flights over time).


## 3. Top Distance Customers Table

- **Content:** Lists customers who have flown the most cumulative distance.
- **Purpose:** Surfaces high-value participants for targeted rewards, marketing, or recognition.


## 4. Top Points Redeemers Table

- **Content:** Ranks customers by total points redeemed.
- **Purpose:** Helps understand redemption behavior; may spotlight highly engaged/loyal users or frequent reward users.


## 5. Top Frequent Flyers Table

- **Content:** Ranks customers by number of flights taken.
- **Purpose:** Detects frequent travelers, who may be business-focused or otherwise critical to program performance.

