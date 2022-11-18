# What factors drive prices of food items?
Author: Craig Gossen

## **Business problem:**
Why are there price fluctuations for similar food items? This model helps relate factors affecting food prices such as the outlet size, location and type. 

Data:
Original data set URL: https://drive.google.com/file/d/1syH81TVrbBsdymLT_jl2JIf6IjPXtSQw/view

![image](https://user-images.githubusercontent.com/114834926/202576796-9bb9f079-2a80-42e0-848b-7e008ffc0adc.png)

## To prepare this data, the data was cleaned, and the following processes were performed:
### Exploratory Data Analysis
- A barplot was created to explore the relationship between the sales and size of store. 
- A histogram was also created to identify trends within item types. 
- A heat map identified potential correlation between the numerical data types. 
![image](https://user-images.githubusercontent.com/114834926/202600244-cba4cc52-3039-45cd-a454-7ed2c6748d8b.png)

***Outlets that sell Fruits and Vegetables, Frozen Foods, and Snack Foods have relatively lower item sales

### Explanatory Data Analysis

- A fun barplot was created to see the differencial of sales of fat vs. non fat dairy. 
- A box plot helped show maximum retail price variations across items. 
- Most interesting, is a scatterplot of sales of the particular product against outlet sales broken out by tier. 
![image](https://user-images.githubusercontent.com/114834926/202600733-c6400bbc-b144-4895-8b30-31cf882c1aed.png)

***Plot indicating Tier 3 outlet sales are higher than the lower tiers. 

## Machine Learning Using the Following Models:
- Linear Regression
- Decision Tree
- Random Forest 

Linear Regression Model (Testing Set):
- R^2: 0.562
- MAE: 847
- MSE: 1,297,558
- RMSE: 1,139

Tuned Decision Tree Regressor Model (Testing Set):
- R^2: 0.6039
- MAE: 762
- MSE: 1,172,122
- RMSE: 1,082

Tuned Random Forest Model (Testing Set):
- R^2: 0.6039
- MAE: 762
- MSE: 1,172,122
- RMSE: 1,082

Analysis: Either the Decision Tree Model or Random Forest Model would be appropriate models to utilize for this data set. Both sets tuned at a depth of 5. 
Using this model to make predictions about the sales of the product in the particular store via various store metric would not be a very reliable due to moderate level of learning achieved shown by R2 of 0.6039. 
