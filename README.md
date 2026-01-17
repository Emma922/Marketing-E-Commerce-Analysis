
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

Revenue per campaing (For more details please visit the dashboard in tableau)
![Campaign Performance](https://github.com/user-attachments/assets/f6076dc5-9578-49ce-a86f-a9156f9c9fb9)


### Category 3 A/B Testing Outcomes

- Variant B is the clear winner, with a conversion rate of 44% compared to 37% (Variant A) and 33% (Control).

- AOV, expected uplift, and segment-level uplift remained equal, meaning the experiment�s impact was limited to conversion efficiency.

- The findings validate Variant B as the most effective treatment, offering a straightforward recommendation to adopt Variant B across campaigns.


![Convertion rate per variant](https://github.com/user-attachments/assets/7bd83755-a21c-4fe9-b197-72077022fd06)


### Category 4 Customer & Product Performance:

- Loyalty tiers: Bronze tier customers contribute the majority of revenue, This hierarchy is inverted compared to the expected loyalty structure, suggesting opportunities for upsell and improvements in the loyalty program improvements.

- Customer segments: Acquisition channel analysis shows that Organic and Paid Search channels bring in the most profitable customers, while Referral customers generate lower revenue, raising efficiency concerns about referral strategies.

- Product categories: Electronics stand as the highest revenue driver, supported by their high AOV. In contrast, Grocery is the lowest performing category with the lowest AOV as well. The tendency shows a clear pattern:the lower the AOV, the lower the revenue contribution

- Margin risks: Discount analysis reveals that no product categories depend heavily on discounts to sell. 

- Higher discount levels correlate with lower revenue. One reason may be that discounted transactions are less common compared to full‑price purchases. 
This imbalance means the effectiveness of discounts cannot be fairly evaluated, as most revenue comes from non‑discounted sales.

![Revenue per product/categories](https://github.com/user-attachments/assets/37aa980d-93cf-49ec-920c-a2925ac0cbc1)

## Recommendations

Based on the analysis, the following actions are recommended to the stakeholder team:

- **Strengthen loyalty programs:** Bronze‑tier customers generate most of the revenue, but higher tiers lag. Upselling and exclusive benefits could increase lifetime value and rebalance the loyalty structure.
- **Scale retention campaigns:** With the highest uplift (~10%), retention initiatives are proven effective. Expanding these campaigns can reduce churn and re‑engage existing customers.
- **Optimize mobile and email strategies:** Mobile devices and email traffic show the strongest conversion rates. Prioritizing mobile UX improvements and targeted email marketing will maximize these strengths.
- **Favor broad targeting approaches:** Campaigns aimed at All Customers and New Customers outperform narrow segments. Broad targeting should be emphasized to capture wider uplift potential.
- **Adopt Variant B across campaigns:** A/B testing confirms Variant B delivers the highest conversion rate. Standardizing this variant will improve efficiency across marketing efforts.
- **Reassess referral strategies:** Referral campaigns underperform in revenue contribution. Revisiting incentives or reallocating resources could improve efficiency.
- **Focus on high‑AOV categories:** Electronics and other high‑value categories should remain a priority, while strategies to improve low‑AOV categories like Grocery can diversify revenue streams.
