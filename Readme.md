# ✈️ Airline Customer Loyalty & Flight Analytics

This comprehensive project analyzes customer loyalty and flight activity data for a fictional airline rewards program. Leveraging Python-based data science techniques, it uncovers trends in customer segments, ticketing behavior, loyalty membership, and point utilization—generating actionable insights to support business strategies around customer retention, segmentation, and maximizing CLV (customer lifetime value).

---

## 📁 Dataset Overview

The project utilizes two core datasets:

### 1. **Customer Loyalty History**
- **Content:** Customer demographics (gender, education, salary, country, city), loyalty card tier (Star, Nova, Aurora), marital status, enrollment/cancellation details, and cumulative CLV.
- **Purpose:** Enables segmentation of customers by value, tenure, and engagement.

### 2. **Customer Flight Activity**
- **Content:** Monthly records for each customer, including total flights, distance flown, points accumulated, points redeemed, and the monetary value of points redeemed.
- **Purpose:** Supports trend analysis over time, customer engagement scoring, and points behavior tracking.

---

## 📊 Project Goals

- **Analyze Enrollment Patterns & Loyalty Trends:**  
  Track sign-up surges, churn rates, and adoption of loyalty card tiers over time.
- **Aggregate & Visualize Flight Activity:**  
  Summarize and plot metrics such as total/mode/median flights, distance, and point redemptions by period and customer cohort.
- **Link Loyalty Status with Activity:**  
  Connect card membership and demographic features to flight and earnings patterns.
- **Deliver Clear Business Insights:**  
  Separate analytics (raw findings) from business-facing interpretations and recommendations.

---

## 🛠 Tools & Libraries

- **Language:** Python 3.x
- **Environment:** Jupyter Notebook (best used with VSCode, JupyterLab, or similar)
- **Libraries:**
  - `pandas` — Data manipulation and aggregation
  - `numpy` — Numerical operations
  - `matplotlib` / `seaborn` — Visualization and plotting
  - `venv` or `conda` — Environment management

---

## 🚀 How to Run

1. **Clone** the repository to your local machine.
2. **Set up your environment:**
python -m venv venv
source venv/bin/activate # For Linux/Mac
or
venv\Scripts\activate # For Windows
3. **Install dependencies:**
pip install -r requirements.txt

4. **Run the Notebooks:**
- Launch Jupyter and open the notebooks in the `notebooks/` directory:
  ```
  jupyter notebook
  ```
- Main analysis and summary visuals can be found in:
  - `notebooks/customer_loyality_eda.ipynb`
  - `notebooks/flight_activity_analysis.ipynb`

---

## 🎯 Typical Use Cases

- **Business Teams:** Identify top-value customers, monitor promotions, understand flight/point dynamics, and design customer retention campaigns.
- **Data Scientists:** Build predictive models for CLV, customer segmentation, churn prediction, and campaign response modeling.
- **Analysts:** Prepare visual insights into the health and evolution of loyalty programs.

---

## 📈 Example Insights

- Discover which cities and loyalty tiers drive the highest CLV.
- Track when and why customers upgrade cards or cancel their memberships.
- Reveal patterns in points earning versus redemption rates and the monetary impact for the airline.

---

## ⚡️ Notes

- Raw datasets are assumed to be located in a `data/` directory.
- Output plots and summary tables are both embedded in the notebooks.
- The project structure separates code, output, and interpretation layers for clarity.

---

## 💬 Feedback & Collaboration

Suggestions or questions? Open an issue or reach out: 
email: hetdave2502@gmail.com
LinkedIn: https://www.linkedin.com/in/hetdave200225/

---

**Happy Analyzing!**
