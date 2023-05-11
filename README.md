# nosql-challenge

The UK Food Standards Agency evaluates various establishments across the United Kingdom, and gives them a food hygiene rating. You've been contracted by the editors of a food magazine, Eat Safe, Love, to evaluate some of the ratings data in order to help their journalists and food critics decide where to focus future articles.

## Part 1: Database and Jupyter Notebook Set Up

  1. Import the data provided in the establishments.json file from your Terminal. Name the database uk_food and the collection establishments. Copy the text you used to import your data from your Terminal to a markdown cell in your notebook.

2. Within your notebook, import the libraries you need: PyMongo and Pretty Print (pprint).

3. Create an instance of the Mongo Client.

4. Confirm that you created the database and loaded the data properly:

5. List the databases you have in MongoDB. Confirm that uk_food is listed.


## Part 2: Update the Database
1. Use NoSQL_setup_starter.ipynb for this section of the challenge.

2. The magazine editors have some requested modifications for the database before you can perform any queries or analysis for them. Make the following changes to the establishments collection:

3. An exciting new halal restaurant just opened in Greenwich, but hasn't been rated yet. The magazine has asked you to include it in your analysis. Add the following information to the database:

4. Find the BusinessTypeID for "Restaurant/Cafe/Canteen" and return only the BusinessTypeID and BusinessType fields.

5. Update the new restaurant with the BusinessTypeID you found.

 6. The magazine is not interested in any establishments in Dover, so check how many documents contain the Dover Local Authority. Then, remove any establishments within the Dover Local Authority from the database, and check the number of documents to ensure they were deleted.

7. Some of the number values are stored as strings, when they should be stored as numbers.

8. Use update_many to convert latitude and longitude to decimal numbers.

9. Use update_many to convert RatingValue to integer numbers.

## Part 3: Exploratory Analysis

1. Eat Safe, Love has specific questions they want you to answer, which will help them find the locations they wish to visit and avoid.

2. Use NoSQL_analysis_starter.ipynb for this section of the challenge.



3. Use count_documents to display the number of documents contained in the result.

4. Display the first document in the results using pprint.

5. Convert the result to a Pandas DataFrame, print the number of rows in the DataFrame, and display the first 10 rows.

6. Which establishments have a hygiene score equal to 20?

7. Which establishments in London have a RatingValue greater than or equal to 4?

8. What are the top 5 establishments with a RatingValue of 5, sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?

9. How many establishments in each Local Authority area have a hygiene score of 0? Sort the results from highest to lowest, and print out the top ten local authority areas.

