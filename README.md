# Cart Abandonment Pattern Analysis

**E-commerce Data Analytics | Cosmetics Retail**

---

## 1. Project Overview

Cart abandonment is one of the common challenges faced by e-commerce businesses. Customers often add products to their shopping carts but leave without completing a purchase.

This project analyses customer shopping events from an anonymised cosmetics online store to identify patterns associated with cart abandonment.

The analysis aims to understand customer shopping behaviour, identify products and brands associated with abandoned carts, estimate the approximate value of abandoned carts, and provide actionable business recommendations.

## 2. Business Problem

The business wants to understand:

- Which products and brands are frequently associated with abandoned carts?
- What shopping behaviours are associated with cart abandonment?
- What percentage of cart sessions result in purchases?
- What is the approximate value associated with abandoned carts?
- Which areas should the business prioritise for improvement?

## 3. Project Objectives

1. Analyse the customer journey from product views to cart additions and purchases.
2. Identify abandoned and converted cart sessions.
3. Analyse abandonment patterns across products and brands.
4. Estimate approximate cart value and at-risk value.
5. Explore shopping behaviour and session duration.
6. Develop evidence-based business recommendations.

## 4. Dataset Information

| Attribute | Details |
|---|---|
| Dataset | eCommerce Events History in Cosmetics Shop |
| Source | Kaggle |
| Publisher | REES46 |
| Business Domain | Cosmetics E-commerce |
| Selected Period | December 2019 |
| File Name | 2019-Dec.csv |
| Data Type | Customer event-level data |

**Dataset provenance:** An anonymised event log published on Kaggle by REES46 for a cosmetics online store.

### Dataset Columns

| Column | Description |
|---|---|
| event_time | Date and time of the event |
| event_type | Customer activity type |
| product_id | Product identifier |
| category_id | Product category identifier |
| category_code | Product category code |
| brand | Product brand |
| price | Product price |
| user_id | Customer identifier |
| user_session | Shopping session identifier |

The raw dataset is stored locally and excluded from this GitHub repository because of its large file size.

## 5. Key Business Metrics

| Metric | Definition |
|---|---|
| Cart Sessions | Sessions containing at least one cart event |
| Converted Cart Sessions | Cart sessions containing a purchase event in the same session |
| Abandoned Cart Sessions | Cart sessions without a purchase event in the same session |
| Cart Abandonment Rate | Abandoned cart sessions / Total cart sessions |
| Cart-Based Conversion Rate | Converted cart sessions / Total cart sessions |
| Approximate Cart Value | Sum of prices recorded in cart events within a session |
| At-Risk Value | Approximate cart value associated with abandoned sessions |
| Session Duration | Time between the first and last event in a session |

**Note:** At-risk value represents the approximate value associated with abandoned carts. It is not guaranteed lost revenue.

## 6. Tools and Technologies

- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- SQL
- Power BI
- Jupyter Notebook
- Git and GitHub

## 7. Project Methodology

The project follows these stages:

1. **Data Understanding:** Examine the dataset structure, columns, event types and initial data quality.
2. **Data Cleaning:** Investigate missing values, duplicates, data types and other quality issues.
3. **Session-Level Analysis:** Identify cart sessions, converted sessions and abandoned sessions.
4. **Exploratory Data Analysis:** Investigate product, brand and customer shopping behaviour patterns.
5. **SQL Analysis:** Calculate business metrics and validate results against Python.
6. **Power BI Dashboard:** Develop an interactive dashboard to communicate findings.
7. **Business Recommendations:** Translate analytical findings into prioritised recommendations.

## 8. Repository Structure

```text
Cart-Abandonment-Analysis-Cosmetics/
|
|-- data/
|   |-- processed/
|       |-- .gitkeep
|
|-- notebooks/
|   |-- 01_data_understanding.ipynb
|
|-- sql/
|   |-- .gitkeep
|
|-- powerbi/
|   |-- .gitkeep
|
|-- reports/
|   |-- .gitkeep
|
|-- README.md
|-- .gitignore
```

The original dataset is maintained locally in `data/raw/` and is intentionally excluded from GitHub.

## 9. Scope and Limitations

- The analysis focuses on one anonymised cosmetics online store and one month of data.
- Checkout-stage information and payment failure details are unavailable.
- Shipping charges, discounts and device information are not available.
- A purchase in a later session may not be counted as a conversion in the original cart session.
- The analysis identifies associations and patterns, not causal relationships.
- Missing brand and category information will be assessed and reported during data cleaning.

## 10. Project Progress

**Status: In Progress**

- [x] Project repository setup
- [x] Dataset selection and acquisition
- [x] Initial data understanding notebook
- [x] GitHub documentation setup
- [ ] Data quality assessment
- [ ] Data cleaning
- [ ] Session-level analysis
- [ ] Exploratory data analysis
- [ ] SQL analysis and validation
- [ ] Power BI dashboard development
- [ ] Business insights and recommendations

## 11. Expected Deliverables

- Cleaned and documented analytical dataset
- Python exploratory data analysis
- SQL queries and validated business metrics
- Interactive Power BI dashboard
- Business insights and prioritised recommendations

---

**Project Purpose:** To demonstrate practical data analytics skills, including data preparation, exploratory analysis, SQL, data visualisation and business problem-solving.