# Cart Abandonment Pattern Analysis



**A Data Analytics Project | E-commerce | Cosmetics Retail**



## Project Overview



Cart abandonment is a common challenge in e-commerce. Customers may add products to their shopping carts but leave without completing a purchase.



This project analyses customer shopping events from an anonymised cosmetics online store to understand which products, brands, and shopping behaviours are associated with cart abandonment.



The goal is to identify patterns, estimate the approximate value associated with abandoned carts, and provide evidence-based recommendations that could help the business improve its cart conversion performance.



## Business Problem



The business wants to understand:



\- Which products and brands are frequently associated with abandoned carts?

\- What shopping behaviours are associated with cart abandonment?

\- What proportion of cart sessions result in purchases?

\- What is the approximate value associated with abandoned cart sessions?

\- Which areas should the business prioritise for further investigation?



## Project Objectives



1\. Analyse the customer shopping journey from product views to cart additions and purchases.

2\. Identify abandoned and converted cart sessions.

3\. Examine product- and brand-level abandonment patterns.

4\. Estimate the approximate cart value and value at risk.

5\. Explore session duration and customer shopping behaviour.

6\. Develop actionable, evidence-based business recommendations.



## Dataset



\- **Source:** An anonymised event log published on Kaggle by REES46.

\- **Business domain:** Cosmetics e-commerce.

\- **Selected period:** December 2019.

\- **File:** `2019-Dec.csv`



The dataset contains event-level records with information such as:



| Column | Description |

|---|---|

| `event\_time` | Date and time of the event |

| `event\_type` | Type of customer activity |

| `product\_id` | Product identifier |

| `category\_id` | Product category identifier |

| `category\_code` | Product category code |

| `brand` | Product brand |

| `price` | Product price |

| `user\_id` | Customer identifier |

| `user\_session` | Shopping session identifier |



**Note:** The raw dataset is stored locally and is not included in this GitHub repository because of its file size.



## Key Business Metrics



| Metric | Definition |

|---|---|

| Cart Sessions | Sessions containing at least one cart event |

| Converted Cart Sessions | Cart sessions containing at least one purchase event in the same session |

| Abandoned Cart Sessions | Cart sessions with no purchase event in the same session |

| Cart Abandonment Rate | Abandoned cart sessions / Total cart sessions |

| Cart-Based Conversion Rate | Converted cart sessions / Total cart sessions |

| Approximate Cart Value | Sum of product prices recorded in cart events within a session |

| At-Risk Value | Approximate cart value associated with abandoned sessions |

| Session Duration | Time between the first and last event in a session |



**Important:** At-risk value is an estimate of the value associated with abandoned carts. It should not be interpreted as guaranteed lost revenue.



## Tools and Technologies



\- Python

\- Pandas

\- NumPy

\- Matplotlib

\- Seaborn

\- SQL

\- Power BI

\- Jupyter Notebook

\- Git and GitHub



## Project Workflow



1\. **Data Understanding:** Inspect the dataset structure, columns, event types, and initial data quality.

2\. **Data Cleaning:** Handle missing values, duplicates, data types, and other data quality issues.

3\. **Session-Level Analysis:** Build session-level data and identify converted and abandoned cart sessions.

4\. **Exploratory Data Analysis:** Investigate abandonment patterns across products, brands, and shopping behaviour.

5\. **SQL Analysis:** Reproduce key business metrics and validate results against Python.

6\. **Power BI Dashboard:** Build an interactive dashboard to communicate business findings.

7\. **Insights and Recommendations:** Present evidence-backed findings and prioritised recommendations.



## Repository Structure



```text

Cart-Abandonment-Analysis-Cosmetics/

â”‚

â”œâ”€â”€ data/

â”‚   â”œâ”€â”€ raw/

â”‚   â””â”€â”€ processed/

â”‚

â”œâ”€â”€ notebooks/

â”‚   â””â”€â”€ 01\_data\_understanding.ipynb

â”‚

â”œâ”€â”€ sql/

â”‚

â”œâ”€â”€ powerbi/

â”‚

â”œâ”€â”€ reports/

â”‚

â”œâ”€â”€ README.md

â””â”€â”€ .gitignore

```



## Scope and Limitations



\- The analysis focuses on one anonymised cosmetics online store and one month of event data.

\- The dataset does not provide checkout-stage details, payment failures, shipping information, or discount information.

\- A purchase occurring in a later session may not be captured as a conversion in the original cart session.

\- The analysis identifies associations and patterns; it does not establish causation.

\- Missing values in product category and brand information will be assessed and reported during data cleaning.



## Project Status



**Currently in progress**



\- \[x] Repository setup

\- \[x] Dataset selection and acquisition

\- \[x] Initial data understanding notebook created

\- \[ ] Data quality assessment and cleaning

\- \[ ] Session-level analysis

\- \[ ] Exploratory data analysis

\- \[ ] SQL analysis and validation

\- \[ ] Power BI dashboard

\- \[ ] Business insights and recommendations



## Expected Deliverables



\- Cleaned and documented analytical data

\- Python exploratory data analysis

\- SQL queries and validated business metrics

\- Interactive Power BI dashboard

\- Business findings and prioritised recommendations



\---



*This project is being developed as a practical portfolio project to demonstrate data analysis, SQL, business understanding, and data visualisation skills.*`n