# nosql-challenge

## Description

This is a 3 part project under the following premise:

The UK Food Standards Agency evaluates various establishments across the United Kingdom, and gives them a food hygiene rating. You've been contracted by the editors of a food magazine, Eat Safe, Love, to evaluate some of the ratings data in order to help their journalists and food critics decide where to focus future articles.

## #Part 1 Database and Jupyter Notebook Set Up

This part is the first portion of the setup before the data analysis with the following steps:

1. Import the data provided in the establishments.json file from Terminal. Name the database uk_food and the collection establishments.

2. Within the notebook, import the neccessary libraries: PyMongo and Pretty Print (pprint).

3. Create an instance of the Mongo Client.

4. Confirm that the database has been created and the data loaded properly:
  - List the databases present in MongoDB. Confirm that uk_food is listed.
  - List the collection(s) in the database to ensure that establishments is there.
  - Find and display one document in the establishments collection using find_one and display with pprint.

5. Assign the establishments collection to a variable to prepare the collection for use.
