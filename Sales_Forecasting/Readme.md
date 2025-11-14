**Objective**<br><br>
The goal of this project is to build a sales forecasting model that predicts the totalamount_local (total sales amount in local currency) based on transactional, customer, and product-level features.

The dataset contains 200,000+ rows representing individual transactions, sourced from multiple sales channels, regions, and products.
Each record corresponds to a unique sales transaction with product, customer, and time-based attributes.
<br><br>
**Data Description** <br><br>

| **Column Name**     | **Description**                                                          | **Type** | 
| ------------------- | ------------------------------------------------------------------------ | -------- | 
| `orderid`           | Unique identifier for each order placed.                                 | `object` | 
| `transactionid`     | Unique identifier for each transaction.                                  | `object` | 
| `productid`         | Unique product code or SKU.                                              | `object` | 
| `productname`       | Name of the product sold.                                                | `object` | 
| `category`          | Product category or business line.                                       | `object` | 
| **`postingdate`**   | Date of Actual transaction posting.                                      | `object` | 
| `year`              | Year of the transaction.                                                 | `int64`  | 
| `month`             | Month of the transaction (1–12).                                         | `int64`  | 
| `dayofweek`         | Day of the week (0–6 or 1–7).                                            | `int64`  | 
| `region`            | Region of the sale (e.g., North, South).                                 | `object` | 
| `country`           | Country of the transaction.                                              | `object` | 
| `company`           | Name of the company (constant across records).                           | `object` | 
| `saleschannel`      | Sales channel (e.g., Online, Retail, Distributor).                       | `object` | 
| `customertype`      | Type of customer (e.g., New, Existing, Corporate).                       | `object` | 
| `customerid`        | Unique identifier for each customer.                                     | `object` | 
| `customername`      | Customer name.                                                           | `object` | 
| `salesrep`          | Sales representative responsible for the transaction.                    | `object` | 
| `plant`             | Production or distribution plant ID.                                     | `object` | 
| `batchno`           | Batch number of the product sold.                                        | `object` | 
| `unitssold`         | Number of units sold.                                                    | `int64`  | 
| **`totalamount_local`** | **Target Variable (Predictor)** — Total sale value in local currency. | `float`  |
| `currency`         | Currency in which the transaction is made                                  | `int64`  | 

Make sure to convert totalamount_local to USD by fetching mapping from CurrencyRates sheet
<br><br>

**Expected Outcome**<br>
- A robust forecasting model capable of predicting future sales (`totalamount_local`) with high accuracy.
- Data-driven insights into seasonality, regional trends, and customer behavior.

**Model Evaluation Criteria**<br>
- **MAPE** (or) **Relevance Evaluation Metrics**
<img width="1606" height="82" alt="image" src="https://github.com/user-attachments/assets/5ab50973-cbc8-4c88-8527-e9ffe5468bd4" />
