
# Marketing & E-Commerce Project

## Project Background
This project leverages a realistic, multi‑table synthetic dataset designed to replicate the analytics environment of a modern e‑commerce company. The dataset simulates customers, products, marketing campaigns, user interaction events, and purchase transactions, providing a rich foundation for end‑to‑end Business Intelligence and Data Science practice.

**Insights and recommendations focus on the following key analytical areas:**

- **Category 1 Funnel & Behavioral Analytics:**  
Comprehensive evaluation of user progression through funnel stages to identify conversion rates, drop-offs, traffic source, and device type impact.

- **Category 2 Campaign Performance:**  
In-depth analysis of marketing campaigns to measure revenue impact, conversion lift, discount effects, and overall profitability.

- **Category 3 A/B Testing Outcomes:**  
Descriptive comparison of control vs. treatment groups to assess conversion, AOV differences, and segment-level uplift.

- **Category 4 Customer & Product Performance:**  
Assessment of customer segments, loyalty tiers, and product-level results to highlight revenue drivers and margin risks.



The python code to make exploratory analysis and cleaning the data can be found here:  
[Python Cleaning and Exploration Code](https://github.com/Emma922/Marketing-E-Commerce-Analysis/blob/main/Marketing_%26_E_Commerce_EDA_cleaning.ipynb)

Targeted SQL queries for various business questions can be found here:  
[SQL Business Questions Queries](https://github.com/Emma922/Marketing-E-Commerce-Analysis/tree/main/SQL%20queries%201)


Interactive Tableau dashboards for business perormance analysis are available here:  
- [Marketing & E-Commerce Dashboard](https://public.tableau.com/app/profile/emmanuel.casta.o/viz/Olist_17646411959020/Dashboard1)
<img width="1799" height="1399" alt="Dashboard 1 (11)" src="https://github.com/user-attachments/assets/c4f152e8-3bb6-4395-8462-49f912b6f4a3" />

## Executive Summary

### Overview of Findings

The analysis shows higher conversion rate (68%) from 'Add to cart' to 'Purchase'. Mobile and Email driving stronger conversions. Retention campaigns deliver the highest uplift, while heavy discounts reduce average order value. A/B testing confirms Variant B outperforms control and Variant A. All and New Customers target segments produce the highest Avg Expected Uplift, while Churn Risk is the lowest. Bronze tier customers contribute the majority of revenue, suggesting opportunities for upsell and improvements in the loyalty program improvements.

Key insights include:

-Conversion rate from Add to Cart to Purchase: 68%

-Email traffic source shows the highest conversion rate (70%), followed by Paid Search (68%)

-Mobile is the most effective device type (55%), ahead of Desktop (47%) and Tablet (38%)

-Retention campaigns deliver the highest expected uplift (~10%)

-Targeting all customers yields stronger average uplift than narrow segments, showing broad campaigns can be impactful

-Affiliate and Paid Search campaigns combine strong uplift with high revenue, making them the most profitable channels

-Variant B performs best, with a conversion rate of 44% compared to 37% (Variant A) and 33% (Control)

-Organic and Paid Search channels bring in the most profitable customers

-Bronze-tier customers contribute the majority of revenue, highlighting upsell and loyalty program opportunities

### Based on these findings, The company would benefit from:

-Strengthening loyalty programs to move Bronze-tier customers into higher tiers and increase lifetime value.

-Scaling retention campaigns, which show the strongest uplift, to reduce churn and re‑engage existing customers.

-Optimizing mobile and email strategies, since they drive the highest conversion rates.

-Leveraging Affiliate and Paid Search channels, which combine strong uplift with high revenue, to maximize profitability.

-Expanding broad targeting campaigns, as they deliver higher average uplift than narrow segmentation.

-Refining discount strategies, reducing reliance on heavy discounts to protect average order value.

---

## Insights Deep Dive

### Category 1 Funnel & Behavioral Analytics

- Conversion rate from 'Add to cart users' to 'Purchase User' 68%

- Email traffic source stands out with the highest conversion rate (70%),
Paid Search is the second performer with 68%

- Organic and Direct traffic source are the lowest effective sources with 22% and 16%.

- Mobile is the most effective device type (55%), followed by desktop (47%) and tablet (38%) of conversion rate percent.

- Segments with lower user-based conversion rates implicitly represent higher abandonment after the add-to-cart stage


![Funnel Chart](https://github.com/user-attachments/assets/ff220519-ae38-4e22-afaa-96503b556aa8)


### Category 2 Campaign Performance

- Retention campaigns show the highest expected uplift (~10%), confirming their effectiveness in re‑engaging customers.

- Targeting all customers yields stronger average uplift than narrow segments, suggesting broad campaigns can be impactful.

- Affiliate and Paid Search campaigns combine strong uplift with high revenue, making them the most profitable channels.

- Churn risk shows the lowest Avg Expected Uplift, making this segment less principal than All and New Customer segments.

- Discount applied exhibits a proportional inverse relationship with Total Revenue and Orders.
Lower discound, higher revenue and orders, being 0 discount the better performing.

- There are no surprises in campaing ratio between 'discounted and non discounted orders'. 
Almost every campaing following a 60%-80% ratio.

![Campaign Performance](https://github.com/user-attachments/assets/f6076dc5-9578-49ce-a86f-a9156f9c9fb9)


### Category 3 A/B Testing Outcomes

- Variant B is the clear winner, with a conversion rate of 44% compared to 37% (Variant A) and 33% (Control).

- AOV, expected uplift, and segment-level uplift remained equal, meaning the experiment�s impact was limited to conversion efficiency.

- The findings validate Variant B as the most effective treatment, offering a straightforward recommendation to adopt Variant B across campaigns.

- Nr. Orders per Customer Viz
  
- This chart shows the dominance of single-purchase customers, which suggests low repeat purchase rates


![Nr. Orders per Customer](https://github.com/user-attachments/assets/8a2627b8-65f8-49cd-aa54-08d71a6871b2)

### Category 4 Customer & Product Performance:

- Loyalty tiers: Bronze tier customers contribute the majority of revenue, This hierarchy is inverted compared to the expected loyalty structure, suggesting opportunities for upsell and improvements in the loyalty program improvements.

- Customer segments: Acquisition channel analysis shows that Organic and Paid Search channels bring in the most profitable customers, while Referral customers generate lower revenue, raising efficiency concerns about referral strategies.

- Product categories: Electronics stand as the highest revenue driver, supported by their high AOV. In contrast, Grocery is the lowest performing category with the lowest AOV as well. The tendency shows a clear pattern:the lower the AOV, the lower the revenue contribution

- Margin risks: Discount analysis reveals that no product categories depend heavily on discounts to sell. 

- Higher discount levels correlate with lower revenue. One reason may be that discounted transactions are less common compared to full‑price purchases. 
This imbalance means the effectiveness of discounts cannot be fairly evaluated, as most revenue comes from non‑discounted sales.

Sales Performance by State (to consult state details and accurate specific information please enter into the dashboard)


![State Performance](https://github.com/user-attachments/assets/fcf24d00-c86a-41f8-8dd3-95a2bdaf5edc)

### Review score and Service Quality

- Several sellers show low average ratings (<3.0), suggesting operational deficiencies such as late shipments, poor handling, or inconsistent service. 
These sellers should be monitored closely and may require training or performance improvement plans.

- Delivery delays significantly reduce customer satisfaction, as evidenced by the lower average review scores for delayed orders.
This reinforces the importance of logistics efficiency and accurate delivery-time estimates.

- Categories with both high sales volume and high review scores represent strong performance areas. 
In contrast, categories with low review scores signal opportunities for targeted service or product improvements.

- Moveis_escritorio is a high-priority category for intervention because it combines low review scores with high order volume, 
meaning a large number of customers are being negatively affected.

- Cama_mesa_banho is another key category: despite being among the highest in revenue and total orders, it also shows one of the lowest average review scores. 
This mismatch indicates a risk of long-term customer dissatisfaction in a high-impact category.

- Seller 7c67e1448b00f6e969d365cea6b010ab stands out as a critical case: despite selling over 1,300 products, 
the seller maintains the lowest average review scores, suggesting severe operational or quality-related issues.

- Improving logistics reliability and monitoring low-performing sellers could significantly raise customer satisfaction across the platform.

### Order payments type

- High-installment sellers vary significantly across product categories. 

- Categories like 'eletrodomesticos_2', 'moveis_decoracao', and 'automotivo' have the highest average installments, suggesting reliance on financing for higher-priced or durable goods.

- Customer financing preferences align with product type, particularly for expensive or long-term purchase items. 


## Recommendations

Based on the analysis, the following actions are recommended to the stakeholder team:

- **Company growth:** Leverage company growth through marketing strategies across Brazil to sustain momentum and expand reach.
- **Seller campaigns:** Sellers-focused campaigns to encourage sales activity, providing training, incentives or
promotional tools to activate inactive sellers.
- **Marketing campaigns:** Marketing campaigns focused on outperforming products and categories
- **Underperforming teams:** Balance freight values for underperforming states to encourage sales in these places
- **Logistic and seller complaints:** Watch out for logistics and seller complaints by strengthening quality control, improving delivery reliablity, and monitoring seller performance.
- **Customer preferences:** Take advantage of customer financing preferences through targeted marketing and financial strategies
- **Customer loyalty and engagement:** Implement customer engagement programs to increase loyalty and repeat purchases
