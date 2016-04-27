Analytics Vidya had one more very interesting hackathon organized.

Problem statement:
A e-commerce sites dataset is shared and the target variable is to identify whether the marketing email was opened or not. 
And if opened, the link in that email was clicked or not.

Here were the values, if i correctly remember -

0 - Email did not open

1 - Email opened but no action taken

2 - Email opened and link was clicked

I secured Rank 57 on private leaderboard.
And a simple XGB model got me that score.

xgboost.ipynb - 
The approach was very simple and here are the details:

1. Read the data into the data frame

2. Create a target variable

3. Tag the test and train data

4. Check if there are null values in any of the columns 

5. Do processing for null values

6. Create dummy variables for categorical variables in data set 

7. Drop the categorical variables (Now, we have all the floats/int in the data set on which machine learning algo can run)

8. Untag the test and train data

9. Generic method to do a cross validation and fit the model and throw out the feature importance

10. Define the classifier

11. Do grid search to improve the model.

12. Write the output test CSV.
