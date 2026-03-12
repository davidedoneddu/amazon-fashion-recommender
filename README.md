# Amazon Fashion Recommender System

This project implements a recommendation system for the **Amazon Fashion dataset** using multiple recommendation techniques.

The goal of the project is to explore and compare different approaches for generating personalized product recommendations based on item features and user interactions.

---

## Overview

Recommender systems are widely used in e-commerce platforms to suggest products that users are likely to be interested in.  

In this project we build a recommendation pipeline that leverages product metadata and machine learning techniques to generate recommendations for fashion items.

The system focuses on **content-based recommendation**, using textual product descriptions to identify similar products.

---

## Dataset

The project uses the **Amazon Fashion dataset**, which contains product information such as:

- product titles
- product descriptions
- categories
- user interactions

The dataset is commonly used for research in recommendation systems.

---

## Methodology

The recommendation pipeline consists of several steps:

### 1. Data preprocessing
- cleaning product metadata
- text normalization
- removing missing or invalid entries

### 2. Feature extraction
Product descriptions are converted into vector representations using **TF-IDF embeddings**.

### 3. Similarity computation
Product similarity is computed using vector similarity metrics.

### 4. Recommendation generation
A **K-Nearest Neighbors (KNN)** approach is used to retrieve similar products.

---

## Technologies Used

- Python
- Pandas
- Scikit-learn
- NumPy
- Matplotlib

---

## Project Structure
