# Big_Data_ETL_2
Note: Original repo would not push.

## Overview

The purpose of this assignment was to conduct an ETL (extract-transfrom-load) on any two publicly available datasets from Amazon reviews. The goal of Part I was to perform the ETL process in the cloud using Google CoLab and then to upload a df to an RDS instance.

## Part I Results

I selected 2 datasets on Amazon Reviews: the kitchen reviews dataset (https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Kitchen_v1_00.tsv.gz) and the grocery reviews dataset (https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Grocery_v1_00.tsv.gz). The former contained 4,880,466 records and the latter contained half as many records at 2,402,458. 
I created the following: a "review_id_df" DataFrame; a "products_df" DataFrame that dropped duplicates in "product_id" and "product_title" columns only; a "customers_df" DataFrame that grouped data on "customer_id" by how many times customers reviewed a product, and a "vine_df" DataFrame with "review_id", "star_rating", "helpful_votes", "total_votes", and "vine" columns. These were all standard transformations and very straightforward; nearly no cleaning was required excepting the dropping of duplicates. 