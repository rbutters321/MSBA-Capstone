# MSBA-Capstone Project - Rachel Butterfield

Project Goal: 

Home Credit will be able to identify if a customer is a safe candidate to lend to, then create a personalized customer loan and repayment plan to be accountable for, resulting in an increase in revenue, improved customer experience, and lower default rates.

Business Problem: 

Home Credit desires to know safe borrowers in a customer base that is unfamiliar with banking and give the customer a plan for successful loan repayment. Lending to those who are more likely to default on loans decreases the profits of Home Credit and results in negative customer experiences.

Analytic Problem: 

The target variable is specificially customers that do have a negative history of repayment to lend to, and postive repayment. Represented in the application_train/test.csv sets of binary where 1 = Not trust worthy borrower (Client with payment difficulties), 0 = Trustworthy borrower (client with good repayment history).

README: Your group's solution to the business problem.

My individual contribution: 

In the inital EDA portion of this project I explored the scope of missing data in the training and test datasets. I examined all the variables in both sets by looking at the total count and percentage of missing values, examining a handful of the variables to see what the values were, identified possible outliers in the data. I also provided some strategic suggestions as to how to manage the missing data as we continue building out model.

In the modeling portion of this project I wrote all the code for the data cleaning and for the Gradient Boosted Tree Model. The modeling process took me between 30-40 hours, which was surprising to me. I vastly underestimated how much time the data cleaning, hyperparameter tuning, and other techinques like oversampling would take me to figure out. 

README: The business value of the solution.

Difficulties that my group encountered along the way:

I think the biggest difficultly my group encountered was trying to bring all of our models together and compare them. It sounds like an uncomplicated task but by the time we compiled them into one document and ran all the models, we didn't have the time to make the needed corrections before the assignment was due. 

What I learned in the project:

I learned a considerable amount working on this project. I've never worked with which a big dataset before that required so much clean-up. Many of the columns contained null values and I had to research what methods I should use to deal with that problem. Most of the coding I've done historically has been done using R. My group wanted to work in python, so I took it as an opportunity to learn more about that coding language. 

The datasets for this project was massive. Trying to pair down the main training set while also joining in some helpful columns from the other datasets was difficult. Initially, overfitting was a big project with my boosted tree model. I was getting an accuracy score of .90+ which I knew wasn't accurate. Oversampling and doing some additional data cleaning helped with that issue. 
