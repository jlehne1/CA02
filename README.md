# CA02
Files for Computer Assignment 2 are included in this repository.  

In this assignment, a trained model is created that can predict the category of emails (spam or not-spam) and compare the accuracy with correct classifications we already know.  There are 702 emails labeled spam or non-spam that make up the training dataset and 260 emails that make up the testing dataset. 

Using sample code and data provided by the professor, the model was created and explained using in-line comments in the code.  

The first step of the assignment was to clean the data where a dictionary was created using a defined function and then non-alpha-numeric and single-aplha-numeric words were removed.  Finally, the dictionary was shrunk to the desired size (3000 most common words) and the ending dictionary was returned at the end of the function

The second step was to extract feature columns and populate their values into a feature matrix, again through using a defined function.  The resulting function uses the file name to determine if an email is spam or not and extracts the training and testing datasets returning a feature dataset and labels.  

Finally, the main program is run.  Calling on the previous two defined functions, a dictionary is made which then allows for the creation of a features matrix and labels.  These are then used to train the model using the model.fit() function and defining the model as GaussianNB().  The test data is scored by running the trained model using the test data.  Lastly, the model performance is printed in terms of an accuracy score.  This concludes the running of the program.
