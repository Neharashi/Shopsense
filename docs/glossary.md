# Domain Terms Glossary — ShopSense

| Term | Meaning |
|---|---|
| RFM | Recency, Frequency, Monetary — a standard way to segment customers by how recently, how often, and how much they buy |
| Freight value | The shipping cost portion of an order |
| Order status | Where an order is in its lifecycle (delivered, shipped, canceled, etc.) |
| Review score | Customer's satisfaction rating (1–5) after receiving an order |
| Churn | A customer who stops purchasing over a defined period |

Datasets:
Orders:Details regarding the order containing:
     *Order_id,customer_id,order_status,order_purchase_timestamp,order_approved_at,order_delivered_carrier_date,order_delivered_customer_date,order_estimated_delivered_date
Customers: Details regarding the customer conatining:
    *customer_id,customer_unique_id,customer_zip_code_prefix,customer_city,customer_state
Order_items:Details regarding the items ordered with:
    *order_id,order_item_id,product_id,seller_id,shipping_limit_date,price,frieght_value
Payments: Details of the payments for the orders with:
    *order_id,payment_sequential,payment_type,payment_installments,payment_values
Reviews: Details of the review of the order with:
    *review_id,order+id,review_score,review_comment_title,review_comment_message,review_creation_date,review_answer_timestamp
Products: Details of the products with:
    *product_id,product_category_name,product_name_length,product_description_length,product_photos_qty,product_weight_g,product_length_cm,product_height_cm,product_width_cm
Category Translation: Details of product category translation with:
    *product_category_name,product_category_name_english