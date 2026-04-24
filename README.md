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




