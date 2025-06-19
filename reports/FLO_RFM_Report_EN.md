
# FLO RFM Analysis - Project Report

## 1. Project Objective
This project aims to segment FLO's omni-channel customers (both online and offline shoppers) based on their past behaviors. The goal is to determine tailored marketing strategies for each segment.

## 2. Dataset
The dataset contains online and offline purchase records from the last two years, including transaction channels, order counts, spend amounts, and dates per customer.

> Note: The dataset is excluded from the GitHub repo due to licensing and confidentiality.

## 3. Method: RFM Analysis
Customers are evaluated using RFM (Recency, Frequency, Monetary) analysis as follows:

- **Recency**: Number of days since the customer's last purchase
- **Frequency**: Total number of purchases
- **Monetary**: Total amount spent

These metrics are scored between 1-5 to derive "RF_SCORE" values.

## 4. Segment Definitions
RFM scores are converted into segments using regex-based rules such as:

- `champions`, `loyal_customers`, `at_Risk`, `hibernating`, `new_customers`, `cant_loose`, etc.
- Each segment represents a distinct behavior pattern (loyalty, risk, new, dormant, etc.)

## 5. Marketing Recommendations (Case Solutions)

### Case A:
To promote a premium-priced women's shoe brand:

- Customers in `champions` and `loyal_customers` segments,
- Who have shopped in the women's category in the last 12 months should be targeted.

### Case B:
For a discount campaign on children's and men's products:

- Customers in the `cant_loose`, `hibernating`, `new_customers` segments,
- Who are interested in men's/children's categories should be targeted.

## 6. Conclusion
This study successfully segments customers based on behavioral patterns, enabling customized marketing actions for each group.

RFM analysis is an effective tool for identifying key customer traits like loyalty, risk of churn, and potential value.

---

**Note**: This report is based on insights gained from the coding project and contains no personal or proprietary data.
