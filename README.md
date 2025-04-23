# Amazon Reviews 2023 Analysis Project

This project processes and analyzes the [Amazon Reviews 2023](https://huggingface.co/datasets/McAuley-Lab/Amazon-Reviews-2023) dataset, a large-scale collection of Amazon product reviews and metadata (200GB+ across 34 categories). The workflow includes data ingestion, cleaning, exploratory analysis (EDA), sentiment classification, recommender systems, and clustering.

## 📁  Dataset Overview
**User Reviews**
- rating (float): User’s rating of the product (1.0–5.0)
- title (str): Title of the user review
- text (str): Text body of the user review
- images (list): URLs or metadata of images in different sizes
- asin (str): ID of the product
- parent asin (str): Parent ID of the product (products with different colors/sizes can share the same parent)
- user id (str): ID of the reviewer
- timestamp (int): Time of the review (Unix time)
- verified purchase (bool): Whether the purchase was verified
- helpful vote (int): Number of helpful votes the review received

**Metadata**
- main category (str): The domain or top-level category
- title (str): Name of the product
- average rating (float): Rating shown on the product page
- rating number (int): Number of ratings for the product
- features (list): Bullet-point features of the product
- description (list): Descriptions of the product (often multi-line)
- price (float): Price in US dollars (at time of crawling)
- images (list): Product images (thumb, large, hi res)
- videos (list): Videos of the product (with title, URL)
- store (str): Store name (where the product is sold)
- categories (list): Hierarchical categories
- details (dict): Product details (materials, brand, sizes, etc.)
- parent asin (str): Parent ID of the product
- bought together (list): Bundles or recommended items often bought together
