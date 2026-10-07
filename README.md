# OmniRetail Customer Satisfaction & Loyalty Analytics

A Power BI analysis of 120 customer feedback records for OmniRetail, a U.S. electronics and smart-home retailer, built to identify what drives satisfaction and loyalty across regions, demographics, and support experiences.

![Dashboard preview](assets/images-preview.png)

## Overview

OmniRetail is a U.S. retail chain selling electronics and smart home products online and in stores. In 2024, the company collected customer feedback combining satisfaction scores, purchasing behavior, demographics, support history, and location data — but had no clear picture of what was actually driving satisfaction and loyalty.

This project analyzes that dataset in Power BI to answer nine core business questions: which factors drive high and low satisfaction, which customer segments and regions are most and least loyal, whether contacting support hurts the relationship, and how loyalty relates to satisfaction overall. The result is a three-page interactive dashboard plus a full written analysis — including one counterintuitive finding that reframes how OmniRetail should think about retention: loyalty and satisfaction aren't driven by the same thing.

## Business Questions

This analysis was built to answer nine questions:

1. What are the main factors contributing to high vs. low satisfaction scores?
2. Are certain customer segments (age, gender, group) more loyal than others?
3. Which locations report consistently high or low satisfaction scores?
4. Does contacting customer support negatively impact satisfaction?
5. How do factors like "Price" or "Product Variety" influence customer loyalty?
6. Do repeat purchasers report higher satisfaction than one-time buyers?
7. What is the relationship between loyalty level and satisfaction score?
8. Do specific demographic groups favor certain satisfaction factors?

## Dashboard

The Power BI report has three pages:

- **Executive Summary** — headline KPIs and a findings panel surfacing the report's key takeaways at a glance
- **Customer Satisfaction (CX Insight)** — satisfaction by factor, the loyalty × satisfaction matrix, and support/buyer-type comparisons
- **Loyalty, Segmentation & Preference (Segments)** — loyalty and factor preference broken down by age group, gender, and customer group, plus state-level satisfaction

## Key Findings

- **Loyalty and satisfaction are not the same thing.** Low-loyalty customers report the *highest* average satisfaction (5.84), while High-loyalty customers average lower (5.65) — loyalty here tracks behavior (likely purchase frequency or tenure), not happiness. Raising satisfaction scores alone won't raise loyalty.
- **Product Variety is a bigger retention risk than Price.** Customers citing Product Variety as their main factor skew 50% Low-loyalty, versus Price, which leans Medium/High.
- **Loyalty varies by gender more than the dashboard's headline suggests.** Men are proportionally more loyal than women (37% vs. 26% High-loyalty), even though the largest single segment is 35-44-year-old women.
- **Texas is a mixed state, not a model one.** It has both the largest customer base and the widest spread of outcomes — the most Excellent *and* the most Very Poor ratings of any state.
- **Repeat buyers are more satisfied at every loyalty tier**, and **contacting support is associated with lower loyalty and lower satisfaction** — both worth acting on directly.

Full write-up, methodology, and chart-by-chart findings for all nine questions are in [`OmniRetail_Analytics_Documentation.docx`](OmniRetail_Analytics_Documentation.docx).

## Data

| Column | Description |
|---|---|
| `Customer_ID` | Unique customer identifier |
| `Group` | Customer classification — A: high-frequency, B: moderate-frequency |
| `Satisfaction_Score` | 1 (very poor) – 10 (excellent) |
| `Age` / `Age_Group` | Age, bucketed into 25-34, 35-44, 45-54, 55-64 |
| `Gender` | Female / Male |
| `Location` | City and State, with latitude/longitude |
| `Buyer_Type` | Repeat Buyer / One-Time Buyer |
| `Support_Contacted` | Yes / No |
| `Loyalty_Level` | Low / Medium / High |
| `Satisfaction_Factor` | Main driver of the score (e.g., Price, Packaging, Product Variety) |

## Tools

- **Power BI** — data modeling, DAX, and dashboard design
- **DAX** — calculated columns (`Age_Group`, `Satisfaction_Level`) and measures

## Repository Structure


├── data/                                     # Source dataset
├── OmniRetail_Analytics_Documentation.docx   # Full analysis write-up
├── assets/                                   # Dashboard screenshots
└── dashboard.pbix                            # Power BI report


## Author

Built by [Joseph Omu].
[LinkedIn](#) · [Portfolio](#)
