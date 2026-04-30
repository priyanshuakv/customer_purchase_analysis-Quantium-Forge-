# Quantium Data Analytics Virtual Experience

## Retail Strategy & Analytics: Trial Store Performance Evaluation

## 📌 Project Overview
**This project focuses on analyzing retail transaction data to evaluate the commercial success of a new store layout. The analysis is divided into two main phases:**

- **Customer Segmentation**: Identifying high-value segments to target for the "Chips" category.

- **Experimentation & Uplift Testing**: Using a "Control-Trial" methodology to determine if layout changes in specific stores (77, 86, and 88) led to a statistically significant increase in sales and customers.

## 🛠️ Data Methodology

1. **Exploratory Data Analysis (EDA) & Data Cleaning:**
- **Outlier Management**: Identified and removed a major wholesale customer (Loyalty Card 226000) who purchased 200 packets of chips in a single transaction, as this skewed retail trends.
- **Product Refinement**: Filtered out non-chip products (e.g., Salsas/Dips) and standardized brand names (e.g., merging "RRD" and "Red Rock Deli").
- **Target Segment Identification**: Discovered that Mainstream Young Singles/Couples are a premium-value segment, with the highest Average Price per Unit ($4.07) and a strong preference for brands like Kettle and Pringles.

2. **Control Store Selection (The Scientific Approach)** 

To accurately measure the trial's impact, I selected "Control Stores" that acted as a baseline for what would have happened without the layout change. Selection was based on a **Composite Similarity Score (50% Correlation / 50% Magnitude):**

- **Correlation:** Ensures the stores share the same seasonal trends.
- **Magnitude:** Ensures the stores have similar sales volumes.
- **Final Matches:** 

- Trial Store 77 $\rightarrow$ Control Store 233
- Trial Store 86 $\rightarrow$ Control Store 
- 155Trial Store 88 $\rightarrow$ Control Store 2373. 

3. **Statistical Uplift Testing**
- **Scaling:** Control store sales were scaled using a pre-trial scaling factor ($Trial Sales / Control Sales$) to align them with trial store baselines.
- **Assessment:** Calculated the Percentage Difference between Trial and Scaled Control performance.
- **Validation:** Conducted t-tests to ensure that the sales increases in March and April were statistically significant at a 95% confidence interval.
## 📈 Key Results & Findings

![Trial Store Chart](/Images/image_5.png)


**Verdict: Store 77 & 88 = Clear Success**

- **Primary Driver:** The data confirms that the layout change acted as a customer magnet. The growth was driven primarily by an increase in Unique Customers (foot traffic) rather than higher spend per transaction.
- **Behavioral Insight:** The new layout effectively "widened the top of the funnel," bringing in shoppers who previously bypassed the category.

## 🚀 Strategic Recommendations

Based on the success of the trial, the following actions are recommended:
1. **National Rollout:** Implement the new layout across the wider store network, prioritizing high-density urban areas.

2. **Product Optimization:** Increase shelf-space for premium brands (Kettle, Doritos, Pringles) in 175g and 134g sizes to cater to the "Mainstream" target demographic.

3. **Localized Strategy:** For stores like 86, monitor local competitive factors to understand why the sales uplift was less consistent than in other locations.

## 🛠️ Tools & Technologies
- **Language:** Python
- **Libraries:** Pandas (Data Wrangling), Matplotlib/Seaborn (Visualization), Scipy (Statistical Testing)
- **Concepts:** Exploratory Data Analysis (EDA), Uplift Testing, Control Store Selection

## 📊 Key Tasks & Insights

### Task 1: Customer Segment Analysis
- **Goal:** Identify which customer segments drive the most chip sales.
- **Key Insight:** "Mainstream - Young Singles/Couples" pay the highest average price per unit ($4.07) and have a large customer base.
- **Recommendation:** Target this segment with premium brands like Kettle and Pringles.

### Task 2: Trial Store Performance
- **Goal:** Measure the impact of a new store layout in three trial stores (77, 86, 88).
- **Methodology:** Selected Control Stores using correlation and magnitude distance metrics.
- **Result:** Store 77 saw a **62.3% uplift** in sales and a **56% increase** in unique customers.
- **Verdict:** The trial was a success; recommended national rollout.

## 📂 Featured Visualizations

![Sales Uplift Line Graph](/Images/image_3.png)

## *NOTE*:
**"The datasets used in this project were provided by Quantium as part of a virtual simulation via Forage. Due to confidentiality, the raw data files are not included in this repository."**