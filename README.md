# 1. Arcstore E-Commerce : Sales Revenue Analysis
> End-to-end analytics project using Python (Google Colab) and Streamlit to identify sales performance and its impact on customer decision-making.
---
**Table of Contents**
1. Business Understanding
2. Overview Data
3. Cloud Environment & Tech Stack
4. Data Wrangling (Gathering, Assessing, Cleaning)
5. Key Findings
6. Visualization & Explanatory Analysis
7. Insights & Strategic Recommendations
---
**1. Business Understanding**
**1.1 Business Background**
   Arcstore is a fictional e-commerce platform (Kaggle dataset: E-Commerce Public Dataset by Olist) sells a wide variety of products by integrating thousands of sellers across multiple industries. It offers over 70 product categories grouped into several main segments, including Furniture & Home Decor, Electronics & Appliances, Health & Beauty, Sports, Leisure & Entertainment, Fashion & Accessories, and Automotive & Tools.
**1.2 Business Problem**
   Management identified two critical problems threatening the platform’s revenue efficiency and sustainability:
- Problem 1 (Unpredictable Revenue Fluctuations): Monthly and annual revenue streams are difficult to forecast without identifying the key drivers behind sales surges or drops.
- Problem 2 (Inefficient Resource & Promotional Allocation): Marketing efforts and budget allocation are unoptimized due to a lack of mapping between high-demand products and slow-moving items.
- Problem 3 (Low Conversion Rates): The company faces low conversion rates and high churn risks due to conventional filters' inability to balance product ratings, sales volume, and logistics delivery reliability.
**1.3 Business Objective**
  |No| Objective | Analysis | 
  | :--- |:---:| ---: | 
  | 1 | Analyzing the month-over-month (MoM) fluctuations in revenue and order volume | Time Series Analysis |
  | 2 | Analyzing and ranking unit sales volume (top-selling vs. slow-moving products) | Product Perform Analysis |
  | 3 | Analyzing the Impact of Product Ratings on Purchase Decisions | Multi-Criteria Score Analysis | |
