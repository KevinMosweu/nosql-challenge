# nosql-challenge

## Description

This is a 3 part project under the following premise:

The UK Food Standards Agency evaluates various establishments across the United Kingdom, and gives them a food hygiene rating. You've been contracted by the editors of a food magazine, Eat Safe, Love, to evaluate some of the ratings data in order to help their journalists and food critics decide where to focus future articles.

## #Part 1: Database and Jupyter Notebook Set Up

This part is the first portion of the setup before the data analysis with the following steps:

1. Import the data provided in the establishments.json file from Terminal. Name the database uk_food and the collection establishments.

2. Within the notebook, import the neccessary libraries: PyMongo and Pretty Print (pprint).

3. Create an instance of the Mongo Client.

4. Confirm that the database has been created and the data loaded properly:

    -List the databases present in MongoDB. Confirm that uk_food is listed.
    
    -List the collection(s) in the database to ensure that establishments is there.
    
    -Find and display one document in the establishments collection using find_one and display with pprint.

5. Assign the establishments collection to a variable to prepare the collection for use.

## #Part 2: Update the Database

This is the second portion of the setup, the magazine requested some changes to the database before any analysis. These are the steps:

1. A new halal restaurant just opened in Greenwich, but hasn't been rated yet. The magazine has asked to have it include it in the analysis. Add the new document to the database.

2. Find the BusinessTypeID for "Restaurant/Cafe/Canteen" and return only the BusinessTypeID and BusinessType fields.

3. Update the new restaurant with the BusinessTypeID you found.

4. The magazine is not interested in any establishments in Dover, check how many documents contain the Dover Local Authority, remove said documents and check again to confirm they were deleted.

5. Some of the number values are stored as strings, when they should be stored as numbers. Convert latitude and longitude to decimal numbers.

## #Part 3:  Exploratory Analysis

This is part contains the analysis. The Magazine has specific questions they want answered. For each question we display the number of documents in the result, display the first document in the results, convert the result to a Pandas DataFrame, print the number of rows in the DataFrame, and display the first 10 rows.

The following are the questions:

1. Which establishments have a hygiene score equal to 20?

2. Which establishments in London have a RatingValue greater than or equal to 4?

3. What are the top 5 establishments with a RatingValue of '5', sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?

4. How many establishments in each Local Authority area have a hygiene score of 0? Sort the results from highest to lowest, and print out the top ten local authority areas.
