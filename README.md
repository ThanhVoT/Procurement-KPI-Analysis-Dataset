# Procurement-KPI-Analysis-Dataset

## Project Background 
As new procurement data from 2022 - 2023 are released into the public, I'm partnering with the Head of Operations to extract inights and deliver recommendations for our stakeholders. **Reflecting on the challenges our suppliers face, cost optimization, quality assurance, and supply chain effiency, this analysis will allow us to take a closer look at the data to provide strategic insights to drive decision-making.**

## Executive Summary 
This dataset contains over 700 real-world purchases orders from the year 2022 - 2023 from big companies to **reflect on challenges like supplier delays, compliance gaps, and defects. Ideal for analyzing supply chain efficiency, cost optimization, and vendor performance.** By analyzing this data, we can apply predictive forecasting, optimize price negotiations, and identify the most effective suppliers. There is a noticeable trend where suppliers like **Delta_Logistics** and **Beta_Supplies** not only have the highest percentage of defective units but are also the two most frequently used suppliers out of the five available. Understanding why customers continue to prefer these suppliers—and how we can leverage this insight—could help us identify opportunities to both reduce costs and increase revenue. This data presents valuable information that can drive more informed, strategic decisions.

## Insights Deep-Dive

### Procurement & Supplier Performance
  - **Office supplies** rank as the top item category for all three suppliers: **Alpha_Inc, Beta_Supplies, and Delta_Logistics.** 
  - Out of the 777 total orders in the dataset, Delta_Logistics is the most frequently used supplier with 171 orders, while Alpha_Inc has the fewest at 141.
  - Although the difference of 30 orders may seem small, it raises the question of why a notable number of customers are choosing other suppliers over Alpha_Inc.
  - The delivery time across all suppliers ranges from as short as 1 day to as long as 20 days. A brief review of the data suggests that **Beta_Supplies** is consistently the supplier associated with the longest delivery time of 20 days.



### Financial Effiency
  - Between 2022 and 2023, Epsilon_Group generated the highest sales revenue among all suppliers, totaling **$9,192,269.28.** In contrast, Alpha_Inc had the lowest sales revenue, bringing in just over **$7 million.**
  - Breaking down the year further, it is clear that Beta_Supplies quarterly revenue significantly improves from 2022 to 2023. Their average improvement per quarter is **$372,388.65.**
  - The only supplier whose total revenue did not change is **Delta_Logistics.** Their quarterly revenue are consistently throughout 2022 and 2023 with very minor changes.
  - These are the suppliers that give the most discount based on **item_category:**
    - Alpha_Inc offers the lowest discounted price for **Electronics** at **$15.56** per unit.
    - Delta_Logistics offers the lowest discounted price for **MRO** at **$15.60** per unit.
    - Alpha_Inc offers the lowest discounted price for **Office Supplies** at **$13.72** per unit.
    - Episilon_Group offers the lowest discounted price for **Packaging** at **$15.06** per unit.
    - Alpha_Inc offers the lowest discounted price for **Raw Materials** at **$15.09** per unit. 


### Quality Control
  - **Delta_Logistics** have the highest defective rate of **41.04%.**
  - **Beta_Supplies & Delta_Logistics** both has the highest percentage of defective units of over **10%.**
  - **Alpha_Inc** has the highest defective ratio of over **35%** on a single order.
  - **Epsilon_Group** is the only supplier with exactly 4 orders, each having a defective rate over **5%.**


### Compliance & Risk
  - Among all suppliers, Delta_Logistics has the highest number of orders at **171**. However, it also has the most non-compliant orders — **67**, which means nearly **40%** of its orders are non-compliant.
  - Continuing with the positive trend, Epsilon_Group and Alpha_Inc has the lowest non_compliant_orders with the total combine of only **12** out of **307.**
  - This should companies an idea of which supplier they should or should not do business with.


## Recommendations


Maximizing Cost Savings
  - **Negotiating prices with suppliers:** Analyze suppliers that gave the most discount on certain items and negotiate with them to minimize spending while maximizing value.
  - **Prioritizing lowest cost over largest discount:** Contrary to believes, suppliers like Delta_Logistics, who offer the highest discount on MRO items, actually have the highest prices compared to competitors. In contrast, Alpha_Inc, despite offering the lowest discount, provides the most competitive pricing at just **$81.68** per unit, whereas Delta_Logistics charges **$93.35** even after the discount.

***

Reducing Risk in Supplier Selection
  - **Choosing the Correct Suppliers:** Suppliers like Alpha_Inc, Gamma_Co, and Epsilon_Group should be prioritized over Beta_Supplies and Delta_Logistics when selecting who to buy from. Out of 183 instances where defective units exceeded 10%, Beta and Delta accounted for 181 of them.
  - **Target Regularly Compliant Suppliers:** Analyze suppliers with a high percentage of non-compliant orders to narrow down the selection pool. This helps minimize the risk of future non-compliance and contributes to cost savings.

***

Analyzing Suppliers' Performance
  - **Focus on High-Performing Supplier:** Prioritize suppliers that showed significant improvement from 2022 to 2023, as this is a sign of customers' trust which can indicate better product quality or more competitive pricing.
  - **Identify Consistent Supplier:** Maintain relationships with suppliers demonstrating consistent performance, as steady demand often indicates reliable product quality and dependable service.
  - **Improve Delivery Efficiency:** Evaluate suppliers with extended delivery times alongside the item categories they frequently delay. This will help minimize wait times and identify which suppliers can reliably fulfill urgent orders.

***


 
## Assumptions
  - **Order Status:** There were 217 orders which were not delivered, they were either **Partially Delivered**, **Pending**, or **Cancelled**. All which requires further examination.
  - **Shift in Supplier Demand:**
    - While customer names are not visible, it’s reasonable to assume that some have already switched suppliers or are likely to do so soon.
    - Epsilon_Group may be a top choice for these customers, as they have the lowest defect rate and generated the highest revenue between 2022 and 2023.
  - **Price Disparities Among Suppliers:** Multiple suppliers offer different prices for the same product types. However, there appears to be a correlation between the size of the discount offered and the actual price of the item.
    - **Choose Suppliers Offering Best Overall Price:** Ideally, we would get the best deals per unit through one supplier so that we dont have to deal with the hassel of negotiating with many. However, that will never be the case so instead, we go for the second best options. With the provided data, we can see which supplier are selling way over the market price and which can give us the best deal.
      - Best Improved: Beta_Supplies average around $370,000 per quarter and are continiously rising.
      - Best Price Per Unit: "show the pictures of all the best price in SQL"
      - Best Overall: Overall, it seem like the best supplier to go with at the momment is Epsilon_Group with their consistent outstanding performance and low defective rate.
