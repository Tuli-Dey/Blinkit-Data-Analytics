# 🛒 Blinkit Multiple Dataset Analysis Project

> Developed a comprehensive **Blinkit Multi-Dataset Analysis Dashboard** using **Looker Studio** consisting of **6** interactive dashboards covering Products, Orders, Customer Feedback, Inventory, Marketing Performance, and Order Items. Analyzed key metrics such as pricing, margins, delivery performance, customer sentiment, stock levels, campaign effectiveness, and revenue generation. Enabled data-driven decision-making by identifying trends, optimizing inventory and marketing strategies, and improving operational efficiency through insightful visualizations.
- End-to-end data analysis across **multiple business functions**
- Visualization of critical metrics such as **profitability, delivery performance, customer sentiment, and ROAS**
- Identification of **patterns, trends, and anomalies** in operations
- Improved **decision-making through interactive dashboards and KPIs**
  
---

# 1. Project Title

Below are the interactive dashboards created in this project -
- Blinkit Products Dataset Analysis Dashboard.
- Blinkit Orders Analysis Dashboard.
- Blinkit Customer Feedback Analysis Dashboard.
- Blinkit Inventory Analysis Dashboard.
- Blinkit Marketing Performance Analysis Dashboard
- Blinkit Order Items Analysis Dashboard

---

# 2. Project Overview

> This project focuses on building a comprehensive analytics solution for Blinkit using multiple datasets. Six interactive dashboards were created in Looker Studio to analyze different business domains including Products, Orders, Customer Feedback, Inventory, Marketing Performance, and Order Items.

The primary objective of this project is to identify trends, patterns, and inefficiencies, enabling better decision-making through data visualization. By integrating data from multiple sources into a unified dashboard system, the project provides a holistic view of business performance and supports optimization of operations, inventory control, and marketing strategies.

---

# 3. File Details

## Raw Data
- **Raw Blinkit Dataset.xlsx** - Raw Dataset before cleaning.
## Cleaned Data
- **Cleaned Blinkit Dataset.xlsx** - Dataset after cleaning process.
## Pivot Analysis
- **Product Pivot Table.xlsx** - Pivot Analysis based on **Category** (Baby Care, Cold Drinks & Juices, Dairy & Breakfast, etc.)
- **Order Pivot Table.xlsx** - Pivot Analysis based on **Payment Mode** (Cash. Card, etc.) & **Delivery Status** (On-Time, Delayed)
- **Customer & Customer Feedback Pivot Table.xlsx** - Pivot Analysis based on **Customer Segment** (New, Premium, etc.) & **Feedback Category** (Delivery, Product Quality, etc.)
- **Inventory Pivot Table.xlsx** - Pivot Analysis based on **Date** (Jan, Feb, etc.)
- **Marketing Performance Pivot Table.xlsx** - Pivot Analysis based on **Channel** (App, Email, etc.)
- **Order Items Pivot Table.xlsx** - Pivot Analysis based on **Quantity** (2,1,3)
## Dashboard
Below are the Dashboard created in **Looker Studio** -
- **Product Dashboard.png** - Screenshot of the Product dashboard.
- **Order Dashboard.png** - Screenshot of the Order dashboard.
- **Customer Dashboard.png** - Screenshot of the Customer dashboard.
- **Inventory Dashboard.png** - Screenshot of the Inventory dashboard.
- **Marketing Dashboard.png** - Screenshot of the Marketing dashboard.
- **Order Items Dashboard.png** - Screenshot of the Order Items dashboard.

  ---

# 4. Data Dictionary

Below are the description of each Columns used in the **Product dataset** -
| Column Name       | Data Type| Description                                                                            |
|-------------------|----------|----------------------------------------------------------------------------------------|
| product_id        | Integer  | Unique values for each column                                                          |
| product_name      | Text     | Name of the products                                                                   |
| category          | Text     | Category of the product (Fruits & Vegetables, Dairy & Breakfast etc.)                  |
| brand             | Text     | Brand name (Aurora LLC, Ramaswamy-Tata, etc.)                                          |
| price             | Integer  | Price of the product                                                                   |
| mrp               | Integer  | Maximum Retail Price of the product                                                    |
| margin_percentage | Integer  | Percentage of profit earned on a product relative to its selling price                 |
| shelf_life_days   | Integer  | Number of days a product remains safe and usable before it expires                     |
| min_stock_level   | Integer  | Minimum quantity of a product that should be maintained to avoid stock shortages       |
| max_stock_level   | Integer  | Maximum quantity of a product that should be kept in inventory to avoid overstocking   |
| profit_amount     | Integer  | Total amount earned after subtracting all costs from the selling price                 |
| expected_margin   | Integer  | Percentage of profit a business aims to earn on a product or sale                      |

Below are the description of each Columns used in the **Order dataset** -
| Column Name       | Data Type| Description                                                                            |
|-------------------|----------|----------------------------------------------------------------------------------------|
| order_id          | Integer  | Unique values for each column                                                          |
| customer_id       | Integer  | Unique values for each column                                                          |
| order_date        | Date     | Date and time when a customer places an order                                          |
| promised_time     | Date     | Date and time when order will be delivered                                             |
| actual_time       | Date     | Date and time when order received                                                      |
|delivery_time_minutes| Integer| Subtraction of actual_time from promised_time                                          |
| delivery_status   | Text     | Status of the delivery (On-Time, Delayed)                                              |
| order_total       | Integer  | Total order value                                                                      |
| payment_method    | Text     | Which method payment has been done                                                     |
| delivery_partner_id| Integer | Unique values for each column                                                          |
| store_id          | Integer  | Unique values for each column                                                          |

Below are the description of each Columns used in the **Customer dataset** -
| Column Name       | Data Type| Description                                                                            |
|-------------------|----------|----------------------------------------------------------------------------------------|
| feedback_id       | Integer  | Unique values for each column                                                          |
| order_id          | Integer  | Unique values for each column                                                          |
| customer_id       | Integer  | Unique values for each column                                                          |
| rating            | Integer  | Review of the product                                                                  |
| feedback _Text    | Text     | Review provided by the customer about their experience                                 |
| feedback_category | Text     | Classification of feedback (delivery, App Experience etc.)                             |
| sentiment         | Text     | Overall emotional tone of the feedback (positive, negative etc.)                       |
| feedback_date     | Date     | The date when the customer feedback was submitted                                      |

Below are the description of each Columns used in the **Inventory dataset** -
| Column Name       | Data Type| Description                                                                            |
|-------------------|----------|----------------------------------------------------------------------------------------|
| product_id        | Integer  | Unique values for each column                                                          |
| Date              | Date     | When stock received of the product                                                     |
| stock_received    | Integer  | Quantity of inventory items received and added to stock during a specific period or transaction |
| damaged_stock     | Integer  | Quantity of inventory items that are defective, broken, or unsellable due to damage    |
| actual_stock_validity| Text  | Checking of stock validity                                                             |

Below are the description of each Columns used in the **Marketing Performance dataset** -
| Column Name       | Data Type| Description                                                                            |
|-------------------|----------|----------------------------------------------------------------------------------------|
| campaign_id       | Integer  | Unique values for each column                                                          |
| campaign_name     | Text     | Name assigned to a specific marketing campaign                                         |
| date              | Date     | The date on which the campaign performance data is recorded                            |
| target_audience   | Text     | Specific customer segment targeted by the campaign                                     |
| channel           | Text     | Platform or medium used to run the campaign (App, Email, SMS, etc.)                    |
| impressions       | Integer  | Total number of times the campaign was displayed to users                              |
| clicks            | Integer  | Number of times users clicked on the campaign                                          |
| conversions       | Integer  | Number of users who completed the desired action                                       |
| spend             | Integer  | Total amount of money spent on running the campaign                                    |
| revenue_generated | Integer  | Total revenue earned from the campaign                                                 |
| roas              | Integer  | Reported return on ad spend (revenue divided by spend)                                 |
| roas_calculated   | Integer  | System-calculated return on ad spend based on actual revenue and spend values          |

Below are the description of each Columns used in the **Order Items dataset** -
| Column Name       | Data Type| Description                                                                            |
|-------------------|----------|----------------------------------------------------------------------------------------|
| order_id          | Integer  | Unique values for each column                                                          |
| Product_id        | Integer  | Unique values for each column                                                          |
| quantity          | Integer  | Number of units of the product ordered                                                 |
| unit_price        | Integer  | Cost of one unit of the product                                                        |
| revenue_logic     | Integer  | Total revenue calculated as quantity multiplied by unit price                          |

---

# 5. Cleaning Notes
Below are the cleaning steps were performed to prepare the dataset into meaningful insights -
- In **Blinkit Order Datadet** I have created one new column called **delivery_time_minutes** to check the order is in **delayed** position or **On-time**. So that firstly I have calculate **(actual_time - promised_time)** and Based on that we have generated another column that is **delivery_status**. The condition of delivery_status is, **if delivery_time_minutes > 0, then Delayed else On-Time**.
- Changed the number format if **order_total** column.

---

# 6. Analytics View
Below are the KPIs used in the **Product Dashboard** -
- Total Buying Cost of the products.
- Total Selling Cost of the products.
- Avg Buying Cost of the products.
- Avg Selling Cost of the products.
- Avg Margin Percentage.
- Avg shelf life calculation in days.
- Avg Min stock of products.
- Avg Max stock of products.
- Avg Profit earned from a product.
- Avg Expected Margin of the product.

Below is the description of the charts used in the dashboard -

- Category wise calculation of Avg Buying Cost, Avg Selling Cost & Avg Profit amount.
- Distribution of Avg Max Stock & Avg Min Stock Level.
- Category wise created one table and visualize Buying Cost, Selling Cost, Margin Percentage & shelf life days.
- Category wise Avg Margin Percentage.

Below are the KPIs used in the **Order Dashboard** -

- Total Order IDs.
- Order Total Amount.
- Maximum Order Total Amount.
- Max Delivery Time in Mins.
- Total Store IDs.

Below is the description of the charts used in the dashboard -

- Count of Order ID by Delivery Status
- Payment Mode wise Total Order calculation.
- Payment Mode wise Delivery time in Minutes calculation.
- Payment Mode wise Total Order id calculation.

Below are the KPIs used in the **Customer Dashboard** -

- Total Feedback IDs.
- Avg Rating of products.
- Total Customer IDs.
- Sum of Order Total.

Below is the description of the charts used in the dashboard -

- Feedback Category wise Avg of Rating.
- Feedback Category wise Count of Feedback ID.
- Customer Segment wise created one table and visualize Count of customer_id & Sum of Order_totals

Below are the KPIs used in the **Inventory Dashboard** -

- Count of Product IDs.
- Total Stock calculation.
- Total Damaged stock calculation.

Below is the description of the charts used in the dashboard -

- Date wise count of Product ID calculation.
- Date wise total stock calculation.
- Date wise total received stock and total damaged stock calculation.

Below are the KPIs used in the **Marketing Performance Dashboard** -

- Sum of impressions.
- Sum of clicks.
- Sum of conversions.
- Total Revenue calculation.
- Sum of spend.
- Avg of roas_calculated.

Below is the description of the charts used in the dashboard -

- Channel wise sum of spend and sum of impressions calculation.
- Distribution of avg of roas_calculated by SUM of clicks.
- Channel wise created one table and visualize Sum of impressions, Sum of clicks, Sum of conversions, Sum of spend, sum of revenue generated, Avg of roas_calculated.
- Avg of roas calculated by Channel and SUM of clicks.

Below are the KPIs used in the **Order items Dashboard** -

- Calculation of total order ID.
- Count of total quantity.
- Sum of total quantity.
- Avg of unit price calculation.
- Total revenue calculation.

Below is the description of the charts used in the dashboard -

- Quantity wise total unit price.
- Distribution of Unit Price by Revenue.
- Quantity wise created one table and visualize unit price &  total revenue calculation.
- Quantity wise Total Revenue calculation.

---

# 7. Dashboard Image

> **Product Dashboard Image**
_________________________________________________________________________________________________________________________________

<img width="1021" height="767" alt="Product Dashboard" src="https://github.com/user-attachments/assets/1e7a7ef8-64af-483d-be60-28453b990792" />

> **Order Dashboard Image**
__________________________________________________________________________________________________________________________________

<img width="1017" height="767" alt="Order Dashboard" src="https://github.com/user-attachments/assets/b1a6c8e6-f3f5-4f21-a8c3-7f835cdc8115" />

> **Customer Dashboard Image**
___________________________________________________________________________________________________________________________________

<img width="1023" height="763" alt="Customer Dashboard" src="https://github.com/user-attachments/assets/a548c0d8-5fc0-4a57-b601-a8778834554b" />

> **Inventory Dashboard Image**
____________________________________________________________________________________________________________________________________

<img width="1025" height="767" alt="Inventory Dashboard" src="https://github.com/user-attachments/assets/2c53fc50-3fe9-4e63-84f8-19e570750d88" />

> **Marketing Performance Dashboard Image**
____________________________________________________________________________________________________________________________________

<img width="1020" height="767" alt="Marketing Performance Dashboard" src="https://github.com/user-attachments/assets/e20208f8-af7f-439c-8703-dd2875651467" />

> **Order Items Dashboard Image**
____________________________________________________________________________________________________________________________________

<img width="1022" height="767" alt="Order Items Dashboard" src="https://github.com/user-attachments/assets/596341ec-22f8-4619-97bb-009b80b90295" />

---






