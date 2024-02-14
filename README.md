# Eat Safe, Love Exploratory Analysis

## Overview

This repository explores the Eat Safe, Love dataset using MongoDB, PyMongo, Jupyter Notebooks, and Pandas. The analysis aims to answer specific questions provided by Eat Safe, Love to help identify establishments for visitation and avoidance.

## Tools Used

- **MongoDB:** Database to store the Eat Safe, Love dataset.
- **PyMongo:** Python driver for MongoDB.
- **Jupyter Notebooks:** Interactive Python notebooks.
- **Pandas:** Python library for data manipulation.
- **pprint:** Python module for pretty-printing complex data structures.

## Resources

- [MongoDB](https://www.mongodb.com)
- [Stack Overflow - Query String in JavaScript](https://stackoverflow.com/questions/901115/how-can-i-get-query-string-values-in-javascript/901144#901144)
- [Stack Overflow - Load Data from MongoDB into Pandas DataFrame](https://stackoverflow.com/questions/17805304/how-can-i-load-data-from-mongodb-collection-into-pandas-dataframe)
- [GeeksforGeeks - MongoDB Comparison Query Operators](https://www.geeksforgeeks.org/mongodb-comparison-query-operators/)
- [DigitalOcean - How to Use Aggregations in MongoDB](https://www.digitalocean.com/community/tutorials/how-to-use-aggregations-in-mongodb)

## Steps

### 1. Setup

- **MongoDB Setup:**
  - Created 'uk_food' database.
  - Loaded dataset into MongoDB.
- **Collection Assignment:**
  - Assigned 'establishments' collection to the 'establishments' variable.

### 2. Exploratory Analysis

#### Question 1: Hygiene Score of 20

- **Query:**
  - Used `count_documents` to find establishments with a hygiene score of 20.
- **Results:**
  - Printed count, first document, and converted results to Pandas DataFrame.

#### Question 2: London Establishments, RatingValue >= 4

- **Query:**
  - Regex query to find London establishments with RatingValue >= 4.
- **Results:**
  - Displayed count, first document, and converted results to Pandas DataFrame.

#### Question 3: Top 5 RatingValue=5, Sorted by Hygiene Score, Near "Penang Flavours"

- **Query:**
  - Searched near specified location for RatingValue=5, sorted by hygiene score.
- **Results:**
  - Displayed establishments meeting the criteria and converted results to Pandas DataFrame.

#### Question 4: Establishments in Each Local Authority with Hygiene Score of 0

- **Query:**
  - Built an aggregation pipeline to find establishments with hygiene score of 0, grouped by Local Authority, and sorted results.
- **Results:**
  - Displayed count, first 10 results, and converted results to Pandas DataFrame.

## Conclusion

This exploratory analysis provides insights into various aspects of the Eat Safe, Love dataset, helping identify establishments based on hygiene scores, ratings, and proximity to specific locations.
