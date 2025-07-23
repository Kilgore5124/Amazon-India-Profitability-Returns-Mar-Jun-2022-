# Project Log: Unlock Profits with E-Commerce Sales Data
### Amazon India | March–June 2022 | Portfolio Project by Charles Kilgore

This project log details every technical and strategic step involved in preparing, analyzing, and visualizing e-commerce sales data for Amazon India. The goal was to extract actionable business insights to optimize profitability and reduce return-related losses.

---

## Data Cleaning Process (Excel)

### Files Used:
- `Amazon Sale Report.csv` → cleaned to `Cleaned_Amazon_Sales_Data.xlsx`

### Steps Taken:
| Step | Action | Reason |
|------|--------|--------|
| 1 | Deleted irrelevant columns (`Fulfilled By`, `Promotion ID`, `Unnamed`) | Columns provided no business value or variation |
| 2 | Extended all column widths | To display hidden date values (Excel was showing `######`) |
| 3 | Verified date ranges | Ensured all orders were within Mar–Jun 2022 scope |
| 4 | Formatted Revenue | Set to `Currency (Custom)` with `₹` prefix for INR |
| 5 | Checked for blank rows and dropped any without critical values | Prevent calculation errors in Tableau |
| 6 | Verified uniqueness of Order ID | Ensured valid count of total orders |
| 7 | Flagged return-related statuses for later segmentation | Used for return volume/type insights |

**Outcome:** Clean, structured dataset ready for Tableau analysis.

---

## KPI Development

| KPI | Formula | Purpose |
|-----|---------|---------|
| Total Revenue | SUM([Order Amount]) | Core profitability metric |
| AOV | SUM([Order Amount]) / COUNTD([Order ID]) | Measures order value trends |
| Total Orders | COUNTD([Order ID]) | Baseline activity |
| Return Rate | Return Orders / Total Orders | Assesses operational efficiency |

All metrics formatted in Tableau using `Currency (Custom)` for ₹ and % as needed.

---

## Tableau Visuals

### Story Slides Created:
1. **Executive Summary** – Project goals, key findings, and recommendations
2. **Revenue by Month** – April peak, followed by decline → need for retention campaigns
3. **Revenue by Category** – Apparel & shoes dominate → bundle & upsell strategy
4. **Top-Selling Styles** – 80/20 distribution → highlight and pair with slower SKUs
5. **Returns by Category** – Shoes & electronics return-heavy → improve fulfillment
6. **Return Types (Pie)** – Damage/rejection dominate → operational fixes needed
7. **Top States by Revenue** – Urban concentration → geo-targeting & regional expansion
8. **Strategic Recap (Text Only)** – Clear call to action for business impact

---

## Key Insights

- Revenue peaked in April → highlight need for sustained marketing
- Top styles account for majority of income → protect and promote them
- Returns heavily affect profit drivers → sizing, packaging, and QA are critical
- Urban states dominate → room to expand into tier-2 regions

---

## Strategic Recommendations

| Area | Recommendation |
|------|----------------|
| Revenue Growth | Use remarketing, bundles, and price tests |
| Return Reduction | Improve sizing tools, packaging, vendor QA |
| Product Strategy | Feature top styles, rotate slower SKUs |
| Regional Strategy | Double down on top states; test new ones |

---

## Tools Used

- **Excel** – Data cleaning, validation
- **Tableau** – KPI dashboards, strategic story
- **GitHub** – Project hosting and version control
- [LinkedIn](https://www.linkedin.com/in/charles-kilgore-250737142)

