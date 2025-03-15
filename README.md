# nosql-challenge
Module 12 Challenge

NoSQL Challenge - UK Food Establishments Database

Overview

This project focuses on collecting, storing, and analyzing food establishment data in the UK using a NoSQL database. The challenge involves setting up a MongoDB database, updating records, and performing exploratory data analysis to derive insights for the "Eat Safe, Love" magazine editors.

Project Structure

NoSQL_setup.ipynb: This notebook is responsible for setting up the NoSQL database (MongoDB), importing data, and verifying the database structure.

NoSQL_analysis.ipynb: This notebook contains queries and data analysis performed on the dataset, extracting meaningful insights.

Data Collection

The dataset used in this challenge includes information about food establishments in the UK, such as business names, locations, food hygiene ratings, and local authority details.

Steps Undertaken

Part 1: Database and Jupyter Notebook Setup

Database Setup:

Imported the establishments.json dataset into MongoDB.

Created a database named uk_food and a collection named establishments.

Verified the database and collection setup by listing existing databases and collections.

Retrieved and displayed a sample document from the collection.

Part 2: Database Updates

Added a New Restaurant:

Inserted a new record for "Penang Flavours," a halal restaurant in Greenwich.

Retrieved the BusinessTypeID for "Restaurant/Cafe/Canteen" and updated the new entry.

Removed Establishments in Dover:

Identified and removed all establishments located in the Dover Local Authority.

Data Cleaning:

Converted longitude and latitude fields from strings to decimal numbers.

Converted RatingValue to integer values.

Part 3: Exploratory Analysis

Performed analytical queries to answer key questions for the magazine editors:

Identified establishments with a hygiene score of 20. The results of this analysis were a count of 41 restaurants with a hygiene score of 20. The first 10 rown of the data frame were then printed out with 28 columns.

Retrieved establishments in London with a RatingValue greater than or equal to 4. The results of this analysis were 33 restaurants in London having a rating value greather than or equal to 4. The results were then put into a DataFrame with 28 columns.

Found the top 5 establishments with a RatingValue of 5, sorted by lowest hygiene score, closest to "Penang Flavours." The results of this analysis found the 5 establishments with a RatingValue of 5, closest to Penang Flavours, which all had hygiene scores of 0. The results were then put into a DataFrame with 5 rows and 28 columns.

Aggregated the number of establishments in each Local Authority area with a hygiene score of 0, sorting results from highest to lowest. For this analysis, I ran a match query to show each Local Authority Name and the number of establishments each of them had a hygiene score of 0. There were 55 unique Local Authorities and the one with the highest number of establishments with a hygiene score of 0 was Thanet. The results were then converted into a DataFrame with 55 rows.

Results & Findings

Successfully stored and retrieved food establishment data using MongoDB.

Cleaned and standardized data for improved analysis.

Identified key insights on food safety ratings and hygiene scores in different regions.