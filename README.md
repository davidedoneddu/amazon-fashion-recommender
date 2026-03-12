![Python](https://img.shields.io/badge/python-3.10-blue)
![Machine Learning](https://img.shields.io/badge/machine-learning-orange)
![Recommender System](https://img.shields.io/badge/recommender-system-green)

# Amazon Fashion Recommendation System

This project explores the design and implementation of different **Recommendation Systems** using the **Amazon Fashion dataset**.

The goal of the project is to analyze user reviews and product metadata in order to build recommendation models capable of suggesting relevant fashion items to users.

The project was developed as part of the course **Metodi Informatici per la Gestione Aziendale** at the **University of Milano-Bicocca**.

---

# Project Overview

Recommender systems are widely used in e-commerce platforms to personalize user experience and improve product discovery.

In this project we analyze a large dataset of **Amazon Fashion product reviews** and build different recommendation approaches based on:

- exploratory data analysis
- data cleaning and filtering
- collaborative filtering techniques

The project focuses on understanding the structure and sparsity of the dataset and building recommendation models on top of filtered interaction data.

---

# Dataset

The project uses the **Amazon Fashion dataset**, which contains:

- user reviews
- product identifiers
- ratings
- timestamps
- helpful vote metrics
- product metadata

Key dataset characteristics:

- ~2.5 million reviews
- rating values between **1 and 5**
- timestamps ranging from **2002 to 2023**

The dataset is highly **sparse**, which is a typical challenge in recommender system design.

---

# Project Workflow

The project follows several steps.

## 1. Exploratory Data Analysis

Initial exploration of the dataset to understand its structure and quality.

Analysis includes:

- dataset structure
- rating distribution
- timestamp distribution
- helpful vote analysis
- detection of missing values
- identification of duplicate reviews

Visualizations are generated using:

- matplotlib
- seaborn

---

## 2. Data Cleaning

Data preprocessing steps include:

- removal of duplicate reviews
- filtering relevant columns
- creation of simplified interaction datasets
- selection of most relevant users and products

Different dataframes are generated during the process:

- **df** → original dataset
- **df_clean_complete** → cleaned dataset without duplicate reviews
- **df_clean** → reduced dataset with essential fields
- **df_final** → filtered dataset used for recommendation

---

## 3. Sparsity Analysis

Since recommendation systems rely on **user-item interactions**, the sparsity of the interaction matrix is analyzed.

Steps include:

- creation of the **user-item matrix**
- evaluation of sparsity levels
- filtering of low activity users and products
- analysis of correlation between items

This step is crucial to make the recommendation models computationally feasible.

---

## 4. Collaborative Filtering

The recommendation system is implemented using **Collaborative Filtering techniques**.

The idea behind collaborative filtering is that:

> users with similar preferences in the past are likely to have similar preferences in the future.

The model analyzes user-item interactions to identify similar users or similar items and generate recommendations.

---

# Technologies Used

The project is implemented in **Python** using the following libraries:

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- json
- io

---

# Repository Structure

amazon-fashion-recommender
│
├── AnalisiAmazonFashion.ipynb
│ Jupyter notebook containing the full analysis and implementation
│
├── REPORT.pdf
│ Final report describing the methodology and results
│
├── Presentation.pdf
│ Project presentation slides
│
└── README.md


---

# Key Challenges

Some of the main challenges encountered during the project include:

- extremely large dataset size
- high sparsity of the interaction matrix
- data cleaning and preprocessing complexity
- filtering strategies for meaningful recommendations

---

# Future Improvements

Possible improvements include:

- hybrid recommender systems
- evaluation metrics
- deep learning recommendation approaches

---

# Author

Davide Doneddu  
University of Milano-Bicocca  
Computer Science
