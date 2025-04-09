# E-Commerce Customer Invoice Dataset

## Overview
This dataset contains anonymized transaction records from a mid-sized Asian e-commerce platform (2019-2024). The data captures 100 sample transactions with details about purchases, customer demographics, and payment methods. Originally collected for customer segmentation analysis, this dataset is ideal for:

- Market basket analysis
- Payment method trends
- Age/gender spending patterns
- Seasonal purchase behavior

## Data Dictionary

| Column | Type | Description | Notes |
|--------|------|-------------|-------|
| `invoice_no` | String | Unique invoice identifier | Format: I[6 digits] |
| `customer_id` | String | Anonymized customer ID | Format: C[6 digits] |
| `gender` | String | Customer gender | Male/Female |
| `age` | Integer | Customer age | Range: 18-69 |
| `category` | String | Product category | 12 categories including Clothing, Electronics, etc. |
| `quantity` | Integer | Number of items purchased | Range: 1-5 |
| `price` | Float | Total transaction amount (USD equivalent) | Rounded to 2 decimals |
| `payment_method` | String | Payment channel | Alipay/WeChat Pay/Card |
| `invoice_date` | String | Purchase date | MM/DD/YYYY format |

## Sample Data (First 10 Rows)

| invoice_no | customer_id | gender | age | category       | quantity | price  | payment_method | invoice_date |
|-----------|-------------|--------|-----|---------------|----------|--------|----------------|--------------|
| I138884   | C241288     | Female | 28  | Clothing      | 5        | 1500.4 | Alipay         | 5/8/2023     |
| I317333   | C111565     | Male   | 21  | Shoes         | 3        | 1800.51| WeChat Pay     | 12/12/2022   |
| I127801   | C266599     | Male   | 20  | Clothing      | 1        | 300.08 | Card           | 9/11/2022    |
| I173702   | C988172     | Female | 66  | Shoes         | 5        | 3000.85| Alipay         | 16/05/2022   |
| I337046   | C189076     | Female | 53  | Books         | 4        | 60.6   | Card           | 24/10/2022   |
| I227836   | C657758     | Female | 28  | Clothing      | 5        | 1500.4 | Alipay         | 24/05/2023   |
| I121056   | C151197     | Female | 49  | Cosmetics     | 1        | 40.66  | Card           | 13/03/2023   |
| I293112   | C176086     | Female | 32  | Clothing      | 2        | 600.16 | Alipay         | 13/01/2022   |
| I293455   | C159642     | Male   | 69  | Clothing      | 3        | 900.24 | Alipay         | 4/11/2022    |
| I326945   | C283361     | Female | 60  | Clothing      | 2        | 600.16 | Alipay         | 22/08/2022   |

## Known Issues
- Date formats use both DD/MM and MM/DD conventions (original system recorded both)
- Price reflects post-discount amounts
- 3.2% of customer_ids appear multiple times (repeat customers)

## Potential Use Cases
1. ​**​RFM Analysis​**​: `invoice_date` + `price` fields enable Recency/Frequency/Monetary scoring
2. ​**​Payment Trends​**​: Compare adoption of Alipay vs WeChat Pay over time
3. ​**​Category Analysis​**​: Identify high-margin product categories

## License
CC BY-NC-SA 4.0 - Please attribute if used in derived works
