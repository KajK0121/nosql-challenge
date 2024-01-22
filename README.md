# nosql-challenge
Module 12 Challenge
# UK Food Ratings Analysis

## Part 1: Database and Jupyter Notebook Set Up

### Import Data
To begin the analysis, the UK Food Standards Agency's ratings data was imported into a MongoDB database named `uk_food` and a collection named `establishments`. The following steps were executed in the terminal:

```bash
mongoimport --db uk_food --collection establishments --file establishments.json
```

### Jupyter Notebook Setup
In the Jupyter Notebook (`NoSQL_setup_starter.ipynb`), the necessary libraries, PyMongo and Pretty Print (pprint), were imported. A Mongo Client instance was created, and the proper loading of data into the database was confirmed by listing the databases and collections, as well as displaying one document from the `establishments` collection.

## Part 2: Update the Database

### Database Modifications
The database was updated to include a new halal restaurant, "Penang Flavours," in Greenwich. The BusinessTypeID for "Restaurant/Cafe/Canteen" was found and assigned to the new restaurant. Additionally, establishments within the Dover Local Authority were removed, and numeric values were converted from strings.

## Part 3: Exploratory Analysis

### Dataset Exploration
In the Jupyter Notebook (`NoSQL_analysis_starter.ipynb`), the dataset was explored to answer specific questions posed by Eat Safe, Love magazine.

1. **Establishments with Hygiene Score Equal to 20:**
   - Count: [Result Count]
   - First Document: [Document Details]
   - Top 10 Rows in DataFrame: [DataFrame Preview]

2. **London Establishments with RatingValue >= 4:**
   - Count: [Result Count]
   - First Document: [Document Details]
   - Top 10 Rows in DataFrame: [DataFrame Preview]

3. **Top 5 Establishments with RatingValue of 5, Sorted by Lowest Hygiene Score, Nearest to "Penang Flavours":**
   - Count: [Result Count]
   - First Document: [Document Details]
   - Top 10 Rows in DataFrame: [DataFrame Preview]

4. **Establishments in Each Local Authority with Hygiene Score of 0:**
   - Count: [Result Count]
   - First Document: [Document Details]
   - Top 10 Local Authority Areas: [List of Local Authorities]

Note: Coercion of non-numeric values to nulls was performed during the database setup. The dataset was also converted to a Pandas DataFrame for ease of analysis.
