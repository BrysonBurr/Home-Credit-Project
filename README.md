# Home Credit Project

## Business problem and Project Objective
Home Credit Group aims to broaden financial inclusion for unbanked populations by providing a positive and safe borrowing experience. The key challenge is accurately predicting which loan applicants will be able to repay their loans. This prediction is critical because:

1. Rejecting good applicants means lost business opportunities
2. Approving high-risk applicants may lead to financial losses and increased default rates.
3. Many potential customers lack conventional credit histories, making traditional scoring methods inadequate

The company currently uses various statistical and machine learning methods to make these predictions but believes there's room for improvement. Therefore, the goal of this notebook is to develop a model that can more accurately identify which clients are capable of repayment, allowing Home Credit to make better-informed lending decisions.

Customer repayment probability will be generated using a supervised machine-learning model. The model will use as inputs data collected on past customers such as application, demographic, and historical credit behavior. The model will use this information to predict the probability that the customers will repay or not repay their loans. 

## My groups solution to the business problem
Our solution to the business problem includes a predictive model that gives reliable risk scores. The model gives a probability output per applicant that Home Credit can use to deny or approve a loan application. The threshold of what probability is acceptable will depend on what Home Credit deems acceptable. Still, we found by lowering the threshold, i.e., saying an application with a default probability of over .1 should be denied, that there were fewer cases of applicants predicted not to default who then defaulted, which is the most costly case for Home Credit. Our solution also includes top predictors for loan default, such as external source mean and credit amount vs. goods ratio, which Home Credit could use to create stricter rules for those predictors.  

## My contribution to the project
My main contribution to the project was in model building. I created two types of models: Decision Tree and Random Forest. I created base models for both and then adjusted them, tuning different hyperparameters. I then analyzed each model I built regarding the business problem while comparing them to other models that had been built. I also was responsible for creating the final predictions for our best model and then submitting it to Kaggle to get our final score. I explained our final model performance and results, worked on the introduction, and described our data preparation steps. 

## Business value of the solution
The solution we found allows Home Credit to predict better who may or may not default when it comes to giving out loans. Home Credit can approve or reject loan applications based on that probability by outputting a probability of default for each applicant. With this model, they will have fewer applicants who are predicted not to default and end up defaulting. By not approving as many risky candidates as possible, Home Credit will save money and increase profits as there will be fewer financial losses due to defaulted loans. 

## Difficulties encountered along the way
The greatest difficulty we encountered along the way was how to deal with missing info. There are a lot of missing values in this dataset, with some columns having over 50% of the data missing. It wasn't easy to decide how much data to keep and what to eliminate. Deciding the best way to impute those missing values was also tricky for modeling purposes. We also had difficulties getting our models created and improving those models. The first iteration of two of our models, logistic regression and random forest, were the top performing. The changes we made, such as hyperparameter tuning or including interaction terms, did not improve the model as we expected, so it wasn't easy to improve on what we had started with. 

## What I learned in the project
The biggest thing I learned in this project was the importance of EDA and data preparation. I hadn't placed much importance on EDA with previous projects I've done, doing little exploration before getting into the modeling stage. However, I spent a lot more time exploring the data with this project. I created many graphs looking into relationships and trying to find outliers or placeholder values. This allowed me early on to see variables that might be important when modeling, as well as multiple outliers and placeholder values. That was valuable information that I would not have learned had I not taken the time to explore the data thoroughly. When it comes to data preparation, I learned how important it is to be thorough, making sure the data is clean for modeling. A lot of work went into ensuring we dealt with missing information, outliers, and correct data types. By doing so, we made sure our data quality was high, meaning we could trust the results we got. Had we not taken the time to ensure our data was clean, we would have had inaccurate results, and it would have been much harder to trust the models we built. 
