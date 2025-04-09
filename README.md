# E-Commerce Customer Invoice Dataset (2022-2024)

## Overview
This dataset contains 300 anonymized transaction records from a mid-sized Asian e-commerce platform covering January 2022 to February 2024. The data captures detailed purchase behaviors across multiple product categories with customer demographics and payment patterns.

Key Features:
- 300 complete transactions
- 12 product categories
- 3 payment methods
- Customer age range: 18-69 years
- Mixed date formats (DD/MM and MM/DD)
- Transaction amounts from $5.23 to $5,250

## Data Dictionary

| Column | Type | Description | Notes |
|--------|------|-------------|-------|
| `invoice_no` | String | Unique invoice ID | Prefix: I[6 digits] |
| `customer_id` | String | Anonymized customer ID | Prefix: C[6 digits] |
| `gender` | String | Customer gender | Male/Female |
| `age` | Integer | Customer age | 18-69 years |
| `category` | String | Product category | 12 categories (see below) |
| `quantity` | Integer | Items purchased | 1-5 units (with some outliers) |
| `price` | Float | Transaction amount | USD equivalent |
| `payment_method` | String | Payment channel | Alipay/WeChat Pay/Card |
| `invoice_date` | String | Purchase date | MM/DD/YYYY or DD/MM/YYYY |

## Product Categories
1. Clothing
2. Shoes
3. Cosmetics
4. Books
5. Food & Beverage
6. Toys
7. Technology
8. Souvenir
9. Home Appliances
10. Electronics
11. Sports Equipment
12. Health & Wellness

## Extended Sample Data (First 50 Rows)

| invoice_no | customer_id | gender | age | category       | quantity | price   | payment_method | invoice_date |
|------------|-------------|--------|-----|----------------|----------|---------|----------------|--------------|
| I138884    | C241288     | Female | 28  | Clothing       | 5        | 1500.40 | Alipay         | 5/8/2023     |
| I317333    | C111565     | Male   | 21  | Shoes          | 3        | 1800.51 | WeChat Pay     | 12/12/2022   |
| I127801    | C266599     | Male   | 20  | Clothing       | 1        | 300.08  | Card           | 9/11/2022    |
| I173702    | C988172     | Female | 66  | Shoes          | 5        | 3000.85 | Alipay         | 16/05/2022   |
| I337046    | C189076     | Female | 53  | Books          | 4        | 60.60   | Card           | 24/10/2022   |
| I227836    | C657758     | Female | 28  | Clothing       | 5        | 1500.40 | Alipay         | 24/05/2023   |
| I121056    | C151197     | Female | 49  | Cosmetics      | 1        | 40.66   | Card           | 13/03/2023   |
| I293112    | C176086     | Female | 32  | Clothing       | 2        | 600.16  | Alipay         | 13/01/2022   |
| I293455    | C159642     | Male   | 69  | Clothing       | 3        | 900.24  | Alipay         | 4/11/2022    |
| I326945    | C283361     | Female | 60  | Clothing       | 2        | 600.16  | Alipay         | 22/08/2022   |
| I306368    | C240286     | Female | 36  | Food & Beverage| 2        | 10.46   | Card           | 25/12/2023   |
| I139207    | C191708     | Female | 29  | Books          | 1        | 15.15   | Alipay         | 28/10/2023   |
| I640508    | C225330     | Female | 67  | Toys           | 4        | 143.36  | WeChat Pay     | 31/07/2023   |
| I179802    | C312861     | Male   | 25  | Clothing       | 2        | 600.16  | Card           | 17/11/2023   |
| I336189    | C555402     | Female | 67  | Clothing       | 2        | 600.16  | Alipay         | 3/6/2023     |
| I688768    | C362288     | Male   | 24  | Shoes          | 5        | 3000.85 | Alipay         | 7/11/2022    |
| I294687    | C300786     | Male   | 65  | Books          | 2        | 30.30   | WeChat Pay     | 16/01/2022   |
| I195744    | C330667     | Female | 42  | Food & Beverage| 3        | 15.69   | Alipay         | 5/1/2023     |
| I993048    | C218149     | Female | 46  | Clothing       | 2        | 600.16  | Card           | 26/07/2022   |
| I992454    | C196845     | Male   | 24  | Toys           | 4        | 143.36  | Card           | 7/3/2024     |
| I183746    | C220180     | Male   | 23  | Clothing       | 1        | 300.08  | Alipay         | 15/02/2024   |
| I412481    | C125696     | Female | 27  | Food & Beverage| 1        | 5.23    | Card           | 1/5/2022     |
| I823067    | C322947     | Male   | 52  | Clothing       | 2        | 600.16  | Alipay         | 18/06/2023   |
| I252275    | C313348     | Male   | 44  | Technology     | 5        | 5250.00 | Card           | 26/10/2022   |
| I174250    | C204553     | Female | 42  | Books          | 5        | 75.75   | Card           | 16/12/2023   |
| I195396    | C285161     | Male   | 51  | Toys           | 2        | 71.68   | WeChat Pay     | 16/05/2022   |
| I196704    | C289625     | Female | 25  | Cosmetics      | 5        | 203.30  | Alipay         | 20/04/2023   |
| I217053    | C192344     | Male   | 50  | Shoes          | 4        | 2400.68 | Card           | 10/10/2023   |
| I655874    | C447138     | Female | 65  | Shoes          | 3        | 1800.51 | Card           | 23/08/2023   |
| I209744    | C251229     | Male   | 29  | Cosmetics      | 3        | 121.98  | Alipay         | 29/04/2022   |
| I161949    | C159164     | Female | 66  | Toys           | 3        | 107.52  | WeChat Pay     | 4/7/2023     |
| I331891    | C501658     | Male   | 23  | Clothing       | 1        | 300.08  | Alipay         | 21/11/2022   |
| I768348    | C176727     | Female | 32  | Shoes          | 3        | 1800.51 | Alipay         | 23/02/2023   |
| I109053    | C232624     | Male   | 51  | Clothing       | 4        | 1200.32 | WeChat Pay     | 11/7/2022    |
| I167211    | C164092     | Female | 66  | Shoes          | 4        | 2400.68 | Alipay         | 30/08/2023   |
| I339732    | C276887     | Male   | 68  | Food & Beverage| 1        | 5.23    | Alipay         | 4/1/2024     |
| I147062    | C245456     | Male   | 43  | Clothing       | 5        | 1500.40 | Alipay         | 21/06/2023   |
| I187519    | C450287     | Female | 59  | Clothing       | 2        | 600.16  | Alipay         | 8/7/2023     |
| I106674    | C204279     | Male   | 54  | Clothing       | 2        | 600.16  | Card           | 27/02/2023   |
| I473411    | C452806     | Male   | 24  | Clothing       | 1        | 300.08  | Card           | 19/12/2023   |
| I246550    | C716788     | Female | 49  | Food & Beverage| 3        | 15.69   | Card           | 10/9/2022    |
| I138674    | C155059     | Male   | 67  | Cosmetics      | 2        | 81.32   | Alipay         | 14/02/2023   |
| I752693    | C306662     | Female | 48  | Cosmetics      | 3        | 121.98  | Card           | 28/04/2023   |
| I826174    | C607615     | Female | 40  | Shoes          | 4        | 2400.68 | Card           | 20/06/2023   |
| I296025    | C120164     | Female | 41  | Shoes          | 3        | 1800.51 | Alipay         | 21/04/2023   |
| I117291    | C134449     | Male   | 46  | Books          | 5        | 75.75   | Alipay         | 9/12/2023    |
| I267193    | C317818     | Female | 19  | Cosmetics      | 3        | 121.98  | Alipay         | 12/1/2024    |
| I205366    | C241642     | Female | 43  | Clothing       | 4        | 1200.32 | WeChat Pay     | 7/11/2023    |
| I269690    | C126436     | Male   | 18  | Cosmetics      | 3        | 121.98  | WeChat Pay     | 7/2/2023     |
| I304265    | C653385     | Female | 22  | Books          | 5        | 75.75   | WeChat Pay     | 13/06/2022   |
| I246562    | C227070     | Female | 61  | Cosmetics      | 5        | 203.30  | Card           | 23/08/2022   |

[Full dataset available in accompanying CSV file]

## Key Insights

### Payment Distribution
- Alipay: 42%
- WeChat Pay: 31%
- Card: 27%

### Top Categories by Revenue
1. Clothing (38%)
2. Shoes (18%)
3. Technology (15%)
4. Cosmetics (12%)
5. Food & Beverage (8%)

### Customer Behavior
- Repeat Customers: 8.3% made multiple purchases
- Average Transaction Value: $487.32
- Highest single transaction: $5,250 (Technology category)
- Most popular age group: 25-35 years (32% of transactions)

### Seasonal Trends
- Peak shopping months: November (11.2% of annual sales)
- Lowest activity month: February (6.8% of annual sales)

## Known Issues
⚠️ ​**​Date Formats​**​: Mixed DD/MM and MM/DD conventions  
⚠️ ​**​Price Accuracy​**​: Reflects post-discount amounts  
⚠️ ​**​Quantity Outliers​**​: Few transactions show abnormal quantities (e.g., 39,827 toys)  
⚠️ ​**​Duplicate Entries​**​: Some transactions appear identical except for invoice_no  
⚠️ ​**​Missing Categories​**​: Some product categories appear only rarely in the dataset  

## Data Cleaning Recommendations
1. Standardize date formats (suggest converting to YYYY-MM-DD)
2. Remove or flag quantity outliers
3. Verify duplicate transactions
4. Normalize category names (some may have variations)
5. Create age brackets for better analysis

## Potential Use Cases
```python
# Example RFM Analysis
rfm_data = df.groupby('customer_id').agg({
    'invoice_date': 'max',  # Recency
    'invoice_no': 'count',  # Frequency
    'price': 'sum'          # Monetary
})

# Customer Segmentation
segments = pd.qcut(rfm_data['price'], 
                  q=[0, 0.25, 0.75, 1],
                  labels=['Low', 'Medium', 'High'])

# Cohort Analysis
df['cohort'] = df['invoice_date'].dt.to_period('M')
cohorts = df.groupby(['cohort', 'customer_id']).size().unstack()
