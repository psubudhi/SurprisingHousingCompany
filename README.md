
# Project Name : Surprise Housing Company
 SurprisingHousingCompany Realestate Case Study

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- Provide general information about your project here.
	A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia.The company is looking at prospective properties to buy to enter the market. You are required to build a regression model using regularisation in order to predict the actual value of the prospective properties and decide whether to invest in them or not.

- What is the background of your project?
	Realestate company want to purchase houses at lower rate and sell with profits. 
	
- What is the business probem that your project is trying to solve?
	Variables are significant in predicting the price of a house, and

	How well those variables describe the price of a house.

- What is the dataset that is being used?
	 Austrelia market survey with past data.(train.csv)
<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

Approach and steps followed in te project:

	1. EDA Analysis and visualizing the data. ( NA fixes, dummies, formating values, transforming with the help of heatmap on co-related columns and analyzing the  subplots. Also find the relation with the target feature SalePrice column)
	2. Removing the features whis has no relation with the target variables manually.
	3. Creating dummies for categorical features.
	4. Removed dummy columns, If a dummy column for a particular category has the same value (either 0 or 1) in 95% or more of the rows in the dataset as they are higlhy imbalanced and does not provide much information. This is done to prevent the model from being biased or misled by a feature.
	5. Normalized, the data  
	6. Split the dataset to train and test data,. 
	7. Feature selection using RFE for getting n features to observe its r2 square , adj r sq and p values.
	8.Reusable Code Block for Cross-validation, Model Building and Model Evaluation
	9. Got the best alpha value for Lasso and Ridege and compared the coefficients.
	10. Verified with various plots for reviewing the correctness of Assumptons.
		Actual vs Predicted
		Histogram of residuals.
		Q-Q Plot
		Residual vs Predicted
		Plot to chekc Non-Linearity.
		Non-Constant variance.
		Residual Bell curve
		Bias-Variance 
		
	Best Alfa:
		
			Ridge 23.101297
			Lasso 0.003352
		
	Top 10 features discovered from the dataset are :
	['1stFlrSF', '2ndFlrSF', 'OverallQual', 'OverallCond', 'YearBuilt',
       'BsmtFinSF1', 'LotArea', 'GarageArea', 'SaleCondition_Partial',
       'SaleCondition_Normal']
	   
## Conclusions

The Redge and Lasso regression helps to find the alpha that is helps to find the coefficients which has lease MSE (mean square error.). Lasso it simplifies further by removing the feature that does not explain much on the target variable.

The assignment give insight into the advanced linear regression, and provides a great opportunity to learn many nitti-gritties associated with real world problems. 

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
Technologies used in the process are.
1. Jupier notebook 6.5.4( Anaconda navigator 2.4.3 suit)
2. Python 3
3. Python libraries like Numpy, Padnas, Matplotlib, Seaborn
4. Windows 10
5. CSV Dataset

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements


Upgrad Team for providing a opportunity to explore the dataset.

References ...

Upgrad Doubt clearing and regular sessions.
Upgrad learning contents.
Python functions form various pyton sites from Google.
Team mates.

## Contact
Created by https://psubudhi.github.io/portfolio/ - feel free to contact me!
