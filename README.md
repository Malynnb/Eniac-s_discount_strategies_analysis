# Eniac Discount Strategy Analysis

## Overview

This project analyzes how discount strategies impact revenue, order volume, and product performance using Eniac's e-commerce sales data.

By combining product, order, and orderline datasets, the analysis evaluates whether discounts effectively drive sales and identifies pricing strategies that maximize business performance.

---

## Business Questions

* How much are products discounted on average?
* Do higher discounts lead to higher revenue?
* Which products and categories benefit most from discounts?
* Are there optimal discount ranges?
* Can some products maintain strong sales performance without significant discounts?

---

## Dataset

The analysis combines data from multiple sources:

| Table      | Description                      |
| ---------- | -------------------------------- |
| Orders     | Customer order information       |
| Orderlines | Product-level order transactions |
| Products   | Product catalog and pricing data |
| Brands     | Product brand information        |

---

## Data Preparation

Several cleaning and validation steps were performed before analysis:

### Product Data

* Removed duplicate SKUs
* Removed duplicate product names
* Dropped unused columns
* Removed invalid price values
* Converted prices to numeric format
* Removed missing values

### Order Data

* Filtered for completed orders only
* Removed incomplete records
* Validated order IDs against transaction data

### Orderline Data

* Removed unnecessary columns
* Converted prices to numeric format
* Removed invalid quantities and prices
* Standardized column names
* Converted dates to datetime format
* Retained only valid orders

### Data Integration

* Merged product and transaction data using SKU identifiers
* Linked orders, products, and orderlines into a unified analytical dataset

---

## Feature Engineering

To measure discount effectiveness, additional variables were created:

| Feature         | Description                                  |
| --------------- | -------------------------------------------- |
| `discount`      | Difference between list price and sale price |
| `discount_pct`  | Percentage discount applied                  |
| `discount_tier` | Discount category used for comparison        |

### Discount Categories

| Tier   | Range  |
| ------ | ------ |
| Low    | < 10%  |
| Medium | 10–25% |
| High   | > 25%  |

---

## Analysis

The project explores:

* Discount distribution across products
* Revenue by discount level
* Product performance under different discount strategies
* Category-level discount effectiveness
* Relationships between discounts and sales outcomes

---

## Key Findings

* Most products were sold with some level of discounting.
* Higher discounts did not consistently generate higher revenue.
* Moderate discount ranges often outperformed aggressive discounts.
* Several products maintained strong performance without heavy discounting.
* Discount effectiveness varied across product categories.
* Product-specific pricing strategies may be more effective than blanket discount policies.

---

## Tools

* Python
* Pandas
* Jupyter Notebook

---

## Skills Demonstrated

`Data Cleaning` • `Data Validation` • `Data Transformation` • `Data Merging` • `Feature Engineering` • `Exploratory Data Analysis` • `Business Analysis` • `Data Storytelling`

---

## Presentation

Presentation available here:

https://prezi.com/view/f7Zwson0MK917JGcmDsi/?referral_token=WiGIBmlnB3FN
