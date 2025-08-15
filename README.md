Analyze and Provide Insights on Amazon Sales Report
-----------------------------------------------------

## Project Overview

This project analyzes Amazon sales transaction data to identify trends, top-selling products, best-performing regions, and fulfilment method efficiency.
The analysis is visualized in an **interactive 4-page Power BI dashboard**, providing actionable insights for improving sales strategies, inventory planning, customer service, and marketing targeting.

---

##  Dataset

**Source:** Amazon sales CSV dataset (provided for analysis)
**Key Fields:**

* **Order Details:** Order ID, Date, Status
* **Product Details:** Category, Size, Quantity, Amount
* **Fulfilment Details:** Fulfilment method, Sales Channel
* **Location Details:** City, State, Postal Code, Country

---

##  DAX Measures Used

DAX
-- Total Sales
Total Sales = SUM('Amazon Sale Report'[Amount])

-- Total Orders
Total Orders = DISTINCTCOUNT('Amazon Sale Report'[Order ID])

-- Total Quantity Sold
Total Quantity = SUM('Amazon Sale Report'[Qty])

-- Average Order Value
Average Order Value = DIVIDE([Total Sales], [Total Orders], 0)



## Dashboard Pages

### **1. Sales Overview**

* Cards:

  * **Total Sales:** ₹78,590,170.25
  * **Total Orders:** \[Calculated in Power BI]
  * **Total Quantity Sold:** \[Calculated in Power BI]
  * **Average Order Value (AOV):** \[Calculated in Power BI]
* Sales trend over time (Line Chart)
* Date, Category, and Fulfilment slicers

### **2. Product & Fulfilment**

* **Top-selling categories:**

  **T-shirts:** ₹39,206,756.65 (**49.93%** of total revenue)
  **Second category:** ₹21,000,000 (**26.73%** of total revenue)
  **Third category:** ₹11,215,104.12 (**14.28%** of total revenue)
  **Top 3 combined contribution:** **90.88%** of total sales
* Fulfilment method comparison (Clustered Column Chart)
* Product details table (Category, Size, Quantity, Sales)

### **3. Geographical & Customer**

* State-wise sales distribution (Map)
* City-wise sales breakdown (Treemap)
* Location details table (State, City, Orders, Sales, Quantity)

### **4. Insights**

* **Top-Selling Categories:**
  T-shirts lead sales at ₹39.2M (49.93%), followed by the second category at ₹21M (26.73%) and the third category at ₹11.21M (14.28%). Together they contribute 90.88% of total sales.

* **Seasonal Sales Trends:**
  Peak sales observed on the highest sales date in April 2022, with a decline toward the end of the month.

* **Best-Performing Regions:**
  The highest sales were from **Karnataka** with ₹72.53M revenue.
  The second highest sales came from **Telangana** with ₹55.79M revenue.
  Together, these two states contribute **16.33%** of total sales.
  Focusing more inventory and marketing in these regions could further increase revenue.

* **Fulfilment Method Efficiency:**
  Amazon Fulfilled orders generated ₹50.0M in total sales.
  They had **40% fewer cancellations** compared to Merchant Fulfilled orders.
  Merchant Fulfilled performed better in **Blazers** and **Trousers**, especially in size-specific or regional demand.
  Overall, Amazon Fulfilled provided more reliable delivery performance, while Merchant Fulfilled dominated niche or region-specific demand.


## Key Insights

* **T-shirts contribute \~49.93%** of total revenue.
* **Top 3 categories contribute \~90.88%** of overall sales.
* Sales peak in April 2022 and dip toward the end of the month.
* Karnataka and Telangana are the best-performing states, contributing 16.33% of total sales.
* Amazon Fulfilled delivers more consistent performance than Merchant Fulfilled, with 40% fewer cancellations.


## Recommendations

Based on the above insights, the following actions are suggested:

1. **Sales Strategy**

   * Launch targeted promotions during low-sales periods to stabilize revenue.
   * Expand product portfolio to reduce over-dependence on T-shirts and top 3 categories.

2. **Inventory Planning**

   * Prioritize stock for T-shirts and top-performing products to avoid stockouts.
   * Allocate extra inventory to Karnataka and Telangana to meet regional demand spikes.

3. **Customer Service**

   * Continue leveraging Amazon Fulfilled for faster, more reliable deliveries.
   * Improve Merchant Fulfilled service levels, especially in high-cancellation regions.

4. **Marketing Targeting**

   * Focus campaigns on Karnataka and Telangana to further grow their already strong sales base.
   * Explore growth opportunities in underperforming states to diversify revenue streams.

