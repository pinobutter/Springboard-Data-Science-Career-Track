![image](https://user-images.githubusercontent.com/94088917/176323838-e9754598-f4d1-4790-8026-cfa696badfae.png)
# Minizing Risk During Loan Application Process

*The idea of marketplace shopping has been steadily increasing in popularity. LendingClub is a disruptor and became the world's largest peer-to-peer lender. From 2007-2018, we can review their accepted loan applicants and look at the data to see which of those applicants either fully paid as agreed or became written off loans. In this project, I will create models to review and help the LendingClub identify some unique features amongst all the accepted applicants and which features possessed for those fully paid and those written off.

## 1. Data

LendingClub is the world’s largest peer-to-peer lending banks.  The original dataset included both accepted and rejected applicants.  For the purpose of this project, we worked with the accepted loan applicant data.  The original Kaggle data was created by Nathan George, or the import report using the Kaggle API click on the links below:

> * [Kaggle Dataset](https://www.kaggle.com/datasets/wordsforthewise/lending-club/metadata)


## 2. Data Cleaning

## 3. Data Cleaning 

Used raw dataset from 2007 to 2018 Q4 as available
Only considered accepted loan applicant data
Look for missing, NaN and fill values
Drop unnecessary features
Drop repeated features
Convert categorical features to dummy variables

* **Problem 1:** This dataset had missing, NaN and fill values.  **Solution:** review each carefully and process as necessary to context of data.

* **Problem 2:** Drop unecessary features. **Solution:** look at heatmap, correlation to loan amount and loan installment.  If no correlation or none that impacts risk decisioning- drop. 

* **Problem 3:** Drop repeated features. **Solution:** At first, some features during EDA will seem to contain the same data.  During Data-preprocessing review in detail and drop the least relevant or keep the most precise information. For example- Grade and Subgrade contained the same information. Subgrade contained precise data at a subgrade context, therefore dropped Grade.

* **Problem 4:** Convert categorical features to dummy variables. **Solution:** 2 Category Features found 1) features correlated to loan characteristics. 2) Featues correlated to the applicant.

<img width="378" alt="image" src="https://user-images.githubusercontent.com/94088917/176325992-f82f5cbc-ac9e-4026-9b3e-0e611d822867.png">


## 4. EDA

Explored wide variety of features and their correlations. Review in detail for features of those applicants that were fully paid and those that were written off. 

<img width="295" alt="image" src="https://user-images.githubusercontent.com/94088917/176325817-53afd951-1ada-4e89-9fac-84ab9a1acf9f.png">


## 5.Model Selection


I chose to work with Logistic Regression, Random Forest Classifier and XGBoost Classifer

<img width="444" alt="image" src="https://user-images.githubusercontent.com/94088917/176326142-92b3255b-1e61-4a4e-85aa-95a048117b8d.png">


## 7. Comparing Model Performance

In the final predictions notebook, the user can enter their user_id number and receive a list of top ten routes recommended to them:

<img width="378" alt="image" src="https://user-images.githubusercontent.com/94088917/176326237-c7c2f4ec-a5c1-404e-a379-ca753078f9c8.png">


## 8. Takeaways and Future Research

* In the future, I would love to spend more time working with deep machine learning for prediction capabilities, wherein LendingClub can take an applicant and filter out the type most likely to default, based on common features.


## 9. Credits

Thanks to Ricardo Alanis-Tamez for his patience, guidance and for being an amazing Springboard mentor.


