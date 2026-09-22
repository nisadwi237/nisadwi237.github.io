# 1. Arcstore E-Commerce : Sales Revenue Analysis
> End-to-end analytics project using Python (Google Colab) and Streamlit to identify sales performance and its impact on customer decision-making.
---
##**Table of Contents** <br>
[1. Business Understanding](1.business-understanding)<br>
[2. Overview Data](2.overview-data)
[3. Cloud Environment & Tech Stack](3.cloud-environment-&-tech-stack)
[4. Data Wrangling (Gathering, Assessing, Cleaning)](4.data-wrangling-(gathering,-Assessing,-cleaning)
[5. Key Findings](key-findings)
[6. Visualization & Explanatory Analysis](visualization-&-explanatory-analysis)
[7. Insights & Strategic Recommendations](insight&-strategic-recommendations)
---
**1. Business Understanding** 


**1.1 Business Background**
   Arcstore is a fictional e-commerce platform (Kaggle dataset: E-Commerce Public Dataset by Olist) sells a wide variety of products by integrating thousands of sellers across multiple industries. It offers over 70 product categories grouped into several main segments, including Furniture & Home Decor, Electronics & Appliances, Health & Beauty, Sports, Leisure & Entertainment, Fashion & Accessories, and Automotive & Tools.

   
**1.2 Business Problem**
   Management identified two critical problems threatening the platform’s revenue efficiency and sustainability:
- Problem 1 (Unpredictable Revenue Fluctuations): Monthly and annual revenue streams are difficult to forecast without identifying the key drivers behind sales surges or drops.
- Problem 2 (Inefficient Resource & Promotional Allocation): Marketing efforts and budget allocation are unoptimized due to a lack of mapping between high-demand products and slow-moving items.
- Problem 3 (Impact of Product Ratings): Evaluating the impact of product ratings on customer purchasing decisions to understand the relationship between product ratings and sales performance.

  
**1.3 Business Objective**
  |No| Objective | Analysis | 
  | :--- |:---:| :---: | 
  | 1 | Analyzing the month-over-month (MoM) fluctuations in revenue and order volume | Time Series Analysis |
  | 2 | Analyzing and ranking unit sales volume (top-selling vs. slow-moving products) | Product Perform Analysis |
  | 3 | Analyzing the Impact of Product Ratings on Purchase Decisions | Rating Score Analysis |

  
**1.4 Key Business Questions** <br>
1. How have e-commerce sales performance and revenue trended over the past year?
2. Which products are the top-selling and slow-moving items?
3. How do product ratings impact customer purchasing decisions?
   
## **2. Overview Data**
Platform: Kaggle
Dataset : `E-Commerce Public Dataset by Olist`
  |Source Table| Description | Analysis | 
  | :--- |:---:| :---: | 
  |Customers.csv | customer data such as names, contact details, and preferences, vital for personalized services and targeted marketing (customer_id,customer_name,customer_email,customer_city,customer_state)|5 |
  | Order Items.csv | Lists individual items within orders, including product details and quantities, aiding in inventory management and order fulfillment. | Product Perform Analysis (order_id,product_id,seller_id,price,freight_value)|5|
  | Orders.csv | Holds comprehensive order data, including customer details, products, and status, serving as a central repository for order management and tracking (order_id,customer_id,order_status,order_purchase_timestamp,order_approved_at)|5|
  |Products.csv|Catalogs product information, such as names, descriptions, and prices, essential for online shopping platforms to showcase and sell items (product_id,product_category,product_name,product_description,product_price) |5|
  |Reviews.csv|Captures customer feedback and ratings for products, aiding in reputation management and influencing purchasing decisions. (review_id,order_id, review_score, review_comment_title, review_comment_message)|5}
  |Sellers.csv|Contains information about sellers, including contact details and performance metrics, crucial for managing vendor relationships and ensuring quality control (seller_id, seller_name,seller_city, seller_state)|4|
   
