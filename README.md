## Background and Overview  
**This project explores what determines low vs. high customer reviews by exploring two main factors, geolocation and sellers, with a supporting variable, delivery time, which includes delivery delay days and approval time hours. This project included SQL for queries and feature engineering, Python (Pandas) for data inspection, Excel for storage of final data, and a Tableau dashboard of sellers' geolocation.**  

The Brazilian E-Commerce Public Dataset by Olist is a Kaggle dataset that includes 9 tables, from customers to orders to sellers. Through relationships, the identity has been made to find the average review scores for all sellers and geolocations. To evaluate whether seller fulfillment speed (approval time and delivery timing) is associated with customer satisfaction, as measured by review scores, across sellers and regions in Brazilian e-commerce. What makes this project challenging is that customer reviews are subjective, there are many outliers due to numerous sellers with very small sample sizes, and other underlying factors.  

[Brazilian E-Commerce Public Dataset](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)  
[Final dataset](https://github.com/ayydanny/Delivery-Performance-Customer-Reviews-in-Olist-Brazilian-E-Commerce-/blob/main/Olist.xlsx)  
[SQL queries/feature engineering + data inspection (Python)](https://github.com/ayydanny/Delivery-Performance-Customer-Reviews-in-Olist-Brazilian-E-Commerce-/blob/main/Olist.ipynb)   
[Tableau dashboard](https://public.tableau.com/app/profile/daniel.lynn/viz/Olist_17688672148010/Dashboard1)  

The dataset consists of 9 tables with over 90,000 customers, 100,000 orders, 3,000 sellers, and 26 states.

**Key Questions**
* Is seller fulfillment speed associated with customer satisfaction in Brazilian e-commerce?
* Do faster-approving and earlier-delivering sellers receive higher customer review scores?
* Are regional differences in customer reviews aligned with differences in approval and delivery timing?

## Executive Summary

This analysis focuses on two factors—seller performance and geolocation—using delivery time as a supporting variable to examine how fulfillment speed relates to customer reviews. We aim to determine whether faster approval and delivery times, based on the estimated delivery date (above average), can enhance customer satisfaction and drive higher reviews. We aim to explore whether faster delivery times can be based on sellers' speed and regional challenges.

**Geolocation**
- Noticeable pattern of higher customer reviews among states with faster approval and delivery times.

**Sellers**
- Sellers with faster approval times see an approximation of 0.2 increase in the customer reviews.
- Sellers with faster delivery times see an approximation of a 0.6 increase in customer reviews.
- Sellers with faster approval and delivery times see an approximation of a 0.7 increase in customer reviews.

**Key Insights**
- Delivery time tends to have a stronger correlation to customer reviews compared to approval time, likely due to two reasons:
  1. Delivery time is based on the estimated date, and when the product is delivered before the delivery date, it may satisfy the customers much more.
  2. Delivery time differs by multiple days, while approval time differs by a few hours, making delivery time a much stronger factor.
- Even though there is an increase in customer reviews, the difference isn't drastic, meaning there are many other factors, along with customer subjective reviews, that play a role in customer reviews.

<img width="1650" height="792" alt="Tableau geolocation" src="https://github.com/user-attachments/assets/a10d999d-0e86-4b9b-90d6-105aa52f3500" />  

<img width="1666" height="577" alt="Sellers dashboard" src="https://github.com/user-attachments/assets/2d8162bb-0746-411f-9af9-b251f753a101" /> 

**Recommendations**  

- **Prioritize delivery reliability over approval speed**  
  Focus operational improvements on delivery performance rather than approval speed, as delivery timing shows a stronger association with customer reviews.

- **Set seller performance benchmarks using delivery timing**  
  Use delivery delay relative to the estimated delivery date as a benchmark metric for seller performance, rather than raw delivery speed alone.

- **Account for regional delivery constraints**  
  Incorporate regional context when evaluating seller performance, as geographic constraints may impact delivery timing and customer expectations.

**Limitations**  

From the findings, it is important to recognize that there are many sellers with smaller sample sizes, customer reviews are subjective, and there are many factors to consider. So, the answers aren't inherently fixed and can be answered in many ways.
