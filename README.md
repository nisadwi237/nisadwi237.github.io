# 1. Arcstore E-Commerce : Sales Revenue Analysis
> End-to-end analytics project using Python (Google Colab) and Streamlit to identify sales performance and its impact on customer decision-making.
---
##**Table of Contents** <br>
[1. Business Understanding](1.business-understanding)<br>
[2. Overview Data](2.overview-data)
[3. Cloud Environment & Tech Stack](3.cloud-environment-&-tech-stack)
[4. Data Wrangling (Gathering, Assessing, Cleaning)](4.data-wrangling-(gathering,-assessing,-cleaning)
[5. Exploratory Data Analysis (EDA)](5.exploratory-data-analysis(EDA))
[6. Key Findings](key-findings)
[7. Visualization & Explanatory Analysis](visualization-&-explanatory-analysis)
[8. Insights & Strategic Recommendations](insight&-strategic-recommendations)
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
  | 2 | Identifying top-selling products to optimize marketing strategies and budget allocation. | Product Perform Analysis |
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
  | Order Items.csv | Lists individual items within orders, including product details and quantities, aiding in inventory management and order fulfillment (order_id,product_id,seller_id,price,freight_value)|5|
  | Orders.csv | Holds comprehensive order data, including customer details, products, and status, serving as a central repository for order management and tracking (order_id,customer_id,order_status,order_purchase_timestamp,order_approved_at)|5|
  |Products.csv|Catalogs product information, such as names, descriptions, and prices, essential for online shopping platforms to showcase and sell items (product_id,product_category,product_name,product_description,product_price) |5|
  |Reviews.csv|Captures customer feedback and ratings for products, aiding in reputation management and influencing purchasing decisions. (review_id,order_id, review_score, review_comment_title, review_comment_message)|5|
  |Sellers.csv|Contains information about sellers, including contact details and performance metrics, crucial for managing vendor relationships and ensuring quality control (seller_id, seller_name,seller_city, seller_state)|4|

## **Cloud Environment & Tech Stack**
Tools:  Python (Pandas, Seaborn, Matplotlib) · Google Colab ·
Deployment : Streamlit

## **Data Wrangling**
1. Gathering Data
   <img width="880" height="218" alt="image" src="https://github.com/user-attachments/assets/327ab3d8-8c11-409b-8bdb-cb0d6cd7d9ce" />
2. Assessing Data
   <img width="847" height="204" alt="image" src="https://github.com/user-attachments/assets/dcb0d735-43f5-48d8-be78-66bd69fc0d64" />
   Assessing terdiri dari :
   1. Menampilkan missing value
   2. Memeriksa duplikasi data
   3. Memeriksa parameter statistik
3. Cleaning Data
   <img width="855" height="214" alt="image" src="https://github.com/user-attachments/assets/69759254-2f1b-4122-a654-cfcdfbf7faa8" />
   Cleaning data terdiri data :
   1. Menangani missing value
   2. Menghapus duplikasi data
   3. Menghitung jumlah nilai unik
   4. Mengubah tipe data

      
## **Exploratory Data Analysis**

## **Key Findings**
EDA conducted in Google Colab with import file csv. [Full notebook](https://colab.research.google.com/drive/1pkpOjJHFtlYj51ButCciIE__inWXYLt1#scrollTo=GmQeQ5YF8DC0)
**Finding 1 - Revenue Growth and Peak Performance**
Graphic of Total Revenue per Month on September 2017-August 2018 <br>
<img width="877" height="459" alt="image" src="https://github.com/user-attachments/assets/8d578d22-6afc-4ced-b409-95dbae9d8ecb" />
<img width="836" height="474" alt="image" src="https://github.com/user-attachments/assets/2755207a-3a12-4820-abe3-a5cab44b1975" />
 
The line chart shows the e-commerce revenue performance throughout the observation period. Revenue reached its peak in November 2017, whereas the lowest revenue was recorded in December 2017.

**The Insight :**
- Significant Decline & Volume Drop: A sharp drop in revenue was accompanied by a decrease in order volume, indicating a noticeable decline in customer purchasing activity. This downturn requires further investigation to identify potential drivers, such as shifting market demand, product performance issues, or operational bottlenecks.
- Consistent Downward Trend (May–August 2018): Between May and August 2018, sales performance displayed a sustained downward trend, signaling a potential low-demand period. To counter this deceleration, targeted engagement strategies—such as tailored promotional campaigns and re-engagement initiatives—are necessary to stimulate customer demand.
  
**Finding 2 - Identifying top-selling products to optimize marketing strategies and budget allocation.**
<img width="2493" height="583" alt="image" src="https://github.com/user-attachments/assets/53faf7e5-06d2-4437-8330-cff3b9cead58" />

The top-selling product category is cama_mesa_banho, while seguros_e_services reflects the lowest customer interest. Each product category presents its own distinct strengths and weaknesses, but overall customer engagement and purchasing demand remain heavily concentrated in cama_mesa_banho.

**The Insight :** 
-Certain categories exhibit low unit turnover despite high availability, signaling the need for inventory re-evaluation and targeted promotional campaigns (e.g., cross-selling or product bundling).

**Finding 3 - High Rating, High Potential: Growth Opportunities for Top-Rated Products** 
<img width="2104" height="585" alt="image" src="https://github.com/user-attachments/assets/545f76cc-3661-411e-908d-0f126cc3524a" />

Top Recommended Category: Based on aggregate customer review scores, the moveis_decoracao (furniture & decor) category is highly recommended due to its superior rating performance. High product quality consistently earns strong customer satisfaction across purchases.
  
**Insight :**
High Growth Potential: Despite a lower total sales volume compared to cama_mesa_banho (bed, bath, & table), these products offer high value and demonstrate strong market competitiveness. With targeted promotional efforts, this category shows strong potential to challenge top-selling products over time.
