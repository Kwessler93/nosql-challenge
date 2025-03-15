# **NoSQL Challenge**  
### *Module 12 Challenge*  

## **NoSQL Challenge - UK Food Establishments Database**  

### **Overview**  
This project focuses on collecting, storing, and analyzing food establishment data in the UK using a **NoSQL database**. The challenge involves setting up a **MongoDB** database, updating records, and performing exploratory data analysis to derive insights for the *Eat Safe, Love* magazine editors.  

---

## **Project Structure**  

- **📂 NoSQL_setup.ipynb** – Sets up the NoSQL database (**MongoDB**), imports data, and verifies the database structure.  
- **📊 NoSQL_analysis.ipynb** – Contains queries and data analysis performed on the dataset, extracting meaningful insights.  

---

## **Data Collection**  

The dataset used in this challenge includes information about food establishments in the UK, such as:  
✔️ **Business names**  
✔️ **Locations**  
✔️ **Food hygiene ratings**  
✔️ **Local authority details**  

---

## **Steps Undertaken**  

### **🔹 Part 1: Database and Jupyter Notebook Setup**  
- Imported the `establishments.json` dataset into **MongoDB**.  
- Created a database named **uk_food** and a collection named **establishments**.  
- Verified the database and collection setup by listing existing databases and collections.  
- Retrieved and displayed a **sample document** from the collection.  

### **🔹 Part 2: Database Updates**  

#### **➤ Added a New Restaurant:**  
✅ Inserted a new record for **"Penang Flavours"**, a halal restaurant in Greenwich.  
✅ Retrieved the `BusinessTypeID` for `"Restaurant/Cafe/Canteen"` and updated the new entry.  

#### **➤ Removed Establishments in Dover:**  
✅ Identified and removed all establishments located in the **Dover Local Authority**.  

#### **➤ Data Cleaning:**  
✅ Converted **longitude** and **latitude** fields from strings to decimal numbers.  
✅ Converted `RatingValue` to integer values.  

### **🔹 Part 3: Exploratory Analysis**  

Performed analytical queries to answer key questions for the magazine editors:  

- **Identified establishments with a hygiene score of 20.**  
  📌 *Results:* 41 restaurants found. Displayed the first 10 rows of the dataset.  

- **Retrieved establishments in London with a `RatingValue ≥ 4`.**  
  📌 *Results:* 33 restaurants identified, stored in a **DataFrame (28 columns).**  

- **Found the top 5 establishments with a `RatingValue = 5`, sorted by lowest hygiene score, closest to "Penang Flavours."**  
  📌 *Results:* 5 establishments found, all with a hygiene score of 0. Stored in a **DataFrame (5 rows, 28 columns).**  

- **Aggregated the number of establishments in each Local Authority area with a hygiene score of 0.**  
  📌 *Results:* 55 unique **Local Authorities** identified. **Thanet** had the highest number of establishments with a hygiene score of 0. Stored in a **DataFrame (55 rows).**  

---

## **Results & Findings**  

✔️ Successfully stored and retrieved food establishment data using **MongoDB**.  
✔️ Cleaned and standardized data for improved analysis.  
✔️ Identified key insights on **food safety ratings** and **hygiene scores** in different regions.  
