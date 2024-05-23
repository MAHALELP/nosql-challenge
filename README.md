# NoSQL Challenge README

## Part 1: Importing Data

To import the data provided in the `establishments.json` file into MongoDB, I used the following command in my Terminal:

```bash
mongoimport --db uk_food --collection establishments --file /Users/mahalel/Desktop/nosql-challenge/Resources/establishments.json --jsonArray
```

Make sure to replace `/Users/mahalel/Desktop/nosql-challenge/Resources/establishments.json` with the actual path to the file on your system.

## Part 2: Updating the Database

In the `NoSQL_setup_starter.ipynb` notebook, I made the following modifications to the database:

1. Added a new halal restaurant, "Penang Flavours," in Greenwich with a pending rating.
2. Found the BusinessTypeID for "Restaurant/Cafe/Canteen" and updated the new restaurant with this BusinessTypeID.
3. Checked and removed any establishments within the Dover Local Authority from the database.

## Part 3: Exploratory Analysis

In the `NoSQL_analysis_starter.ipynb` notebook, I answered the following questions about the dataset:

1. Identified establishments with a hygiene score equal to 20.
2. Found establishments in London with a RatingValue greater than or equal to 4.
3. Determined the top 5 establishments with a RatingValue of 5, sorted by lowest hygiene score, nearest to the new restaurant, "Penang Flavours."
4. Calculated the number of establishments in each Local Authority area with a hygiene score of 0 and sorted the results from highest to lowest.

For each question, I displayed the number of documents, the first document in the results, and converted the results to a Pandas DataFrame, displaying the number of rows and the first 10 rows.

This README summarizes the steps I took to import the data, update the database, and perform exploratory analysis on the dataset.
