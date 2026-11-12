# DS 4115: Marketing Analytics — Lab 2
## Exploratory Data Analysis (EDA) & Digital Conversion Funnel Analysis using Python

### Overview
This repository contains the completed Jupyter/Kaggle Notebook for **Lab 2 (DS 4115)**[cite: 1]. The project transitions from spreadsheet analytics to a programmatic Python workflow to analyze synthetic GA4-style digital telemetry logs (`ga4_sample_session_logs.csv`), build a 3-step conversion funnel, clean missing records, and identify conversion blockers using correlation heatmaps[cite: 1].

### Objectives Completed
- **Synthetic Data Generation:** Generated 5,000 realistic user session records (`session_id`, `user_id`, `device_category`, funnel flags, `page_views`, and `time_on_site_sec`) using NumPy and Pandas[cite: 1].
- **Conversion Funnel Analysis:** Calculated user session volumes and conversion rates across three stages (`session_start` → `add_to_cart` → `purchase`)[cite: 1].
- **Data Cleaning & Imputation:** Detected and handled missing values in `time_on_site_sec` using median imputation and standardized categorical text formatting[cite: 1].
- **Correlation Heatmap & Insights:** Generated a Seaborn correlation heatmap to evaluate the relationship between user engagement (`page_views`, `time_on_site_sec`) and purchase conversion[cite: 1].

### Key Findings
1. **Cart-to-Purchase Driver:** `add_to_cart_flag` shows a strong positive correlation (**~0.68**) with `purchase_flag`, making cart addition the primary conversion milestone.
2. **Engagement vs. Conversion:** While `page_views` and `time_on_site_sec` correlate strongly with each other (**~0.76**), both show near-zero correlation (**~0.00–0.02**) with purchase conversion—indicating potential UX or checkout friction rather than low engagement.

### Repository Contents
- `Lab2_Conversion_Funnel_EDA.ipynb` — Complete Python notebook with code, outputs, funnel table, and correlation heatmap[cite: 1].
- `ga4_sample_session_logs.csv` — Generated synthetic GA4 session dataset (5,000 rows)[cite: 1].

### Tools & Libraries Used
- **Environment:** Kaggle Notebook / Jupyter Notebook[cite: 1]
- **Libraries:** `pandas`, `numpy`, `matplotlib`, `seaborn`[cite: 1]
