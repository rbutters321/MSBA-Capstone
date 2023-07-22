# MSBA-Capstone Project - Rachel Butterfield

## Project Goal: 

Home Credit will be able to identify if a customer is a safe candidate to lend to, then create a personalized customer loan and repayment plan to be accountable for, resulting in an increase in revenue, improved customer experience, and lower default rates.

## Business Problem: 

Home Credit desires to know safe borrowers in a customer base that is unfamiliar with banking and give the customer a plan for successful loan repayment. Lending to those who are more likely to default on loans decreases the profits of Home Credit and results in negative customer experiences.

## Analytic Problem: 

The target variable is specificially customers that do have a negative history of repayment to lend to, and postive repayment. Represented in the application_train/test.csv sets of binary where 1 = Not trust worthy borrower (Client with payment difficulties), 0 = Trustworthy borrower (client with good repayment history).

## Solution to the business problem:

My group's solution to the business problem was to identify the 5-10 important features of their data that would determine if a customer was likely to default or not. The top 10 features included -

-EXT_SOURCE_3 

-EXT_SOURCE_2 

-AMT_REQ_CREDIT_BUREAU_DAY 

-FLAG_EMP_PHONE 

-FLAG_DOCUMENT_3 

-FLAG_DOCUMENT_16 

-REGION_RATING_CLIENT_W_CITY

-AMT_GOODS_PRICE 

-AMT_REQ_CREDIT_BUREAU_HOUR 

-REG_CITY_NOT_LIVE_CITY

Based on these results, the customer is most likely to default when -

-Have a high number of enquiries to Credit Bureau about the client one day before application

-Client provided work phone

-Suggests that the quality of region is a strong indicator of whether a customer will default. Less rated regions may have more likelihood of default.

-Higher price of goods that the loans were given. 

-Higher number of enquiries to Credit Bureau about the client on hour before

-If the permanent address does not match the contact address then they are more likely to default. 

## The business value of the solution:

To put this data into practical use, to determine whether a customer may default before meeting with an appointment they could be asked survey questions about each of these behaviors. Before a loan is approved, loan officers can consider reviewing this information and setting certain criterias that when met will flag the customer as likely to default, hence the loan officer not approving the loan to the customer. 

## My individual contribution: 

In the inital EDA portion of this project I explored the scope of missing data in the training and test datasets. I examined all the variables in both sets by looking at the total count and percentage of missing values, examining a handful of the variables to see what the values were, identified possible outliers in the data. I also provided some strategic suggestions as to how to manage the missing data as we continue building out model.

In the modeling portion of this project I wrote all the code for the data cleaning and for the Gradient Boosted Tree Model. The modeling process took me between 30-40 hours, which was surprising to me. I vastly underestimated how much time the data cleaning, hyperparameter tuning, and other techinques like oversampling would take me to figure out. 

## Difficulties that my group encountered along the way:

I think the biggest difficultly my group encountered was trying to bring all of our models together and compare them. It sounds like an uncomplicated task but by the time we compiled them into one document and ran all the models, we didn't have the time to make the needed corrections before the assignment was due. 

## What I learned in the project:

I learned a considerable amount working on this project. I've never worked with which a big dataset before that required so much clean-up. Many of the columns contained null values and I had to research what methods I should use to deal with that problem. Most of the coding I've done historically has been done using R. My group wanted to work in python, so I took it as an opportunity to learn more about that coding language. 

The datasets for this project was massive. Trying to pair down the main training set while also joining in some helpful columns from the other datasets was difficult. Initially, overfitting was a big project with my boosted tree model. I was getting an accuracy score of .90+ which I knew wasn't accurate. Oversampling and doing some additional data cleaning helped with that issue. Overall, I feel like the model I built was sufficient at meeting the business and analytics problems of this project. I also recognized that it also had a lot of room for improvement. Given more time I would have liked to learn more about feature enigeering. 
