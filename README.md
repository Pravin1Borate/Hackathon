![alt text](https://github.com/Pravin1Borate/Hackathon/blob/main/images/vidhya.jpeg "Logo Title Text 1")

# Hackathon
Detials of Hackthons:

# 1. Big Mart Sales Prediction
Sales Prediction for Big Mart Outlets
The data scientists at BigMart have collected 2013 sales data for 1559 products across 10 stores in different cities. Also, certain attributes of each product and store have been defined. The aim is to build a predictive model and predict the sales of each product at a particular outlet.

Using this model, BigMart will try to understand the properties of products and outlets which play a key role in increasing sales.

Please note that the data may have missing values as some stores might not report all the data due to technical glitches. Hence, it will be required to treat them accordingly. \
**Data Dictionary**
We have train (8523) and test (5681) data set, train data set has both input and output variable(s). You need to predict the sales for test data set. \
**Evaluation Metric**
Your model performance will be evaluated on the basis of your prediction of the sales for the test data (test.csv), which contains similar data-points as train except for the sales to be predicted. Your submission needs to be in the format as shown in sample submission.
We at our end, have the actual sales for the test dataset, against which your predictions will be evaluated. We will use the Root Mean Square Error value to judge your response.

[Please checkout the notebook for the result and approch](https://github.com/Pravin1Borate/Hackathon/blob/main/Big%20Mart%20Sales%20Prediction/Big%20Mart%20Sales%20Prediction.ipynb)

For the above hackthon total **42320** people current rank for is **740**

**Approch:**
1. Item_Weight and Outlet_Size have some missing values in the data so by cheking outlier imputed with mean values. For outlet_size is categorical variable so imputed with mode.
2. Later by doing some visualization came with some interesting insight of data. Like which item mostly having most sales so shop owner can purchaes that item in much quantity.
3. Implemented Base model by using linear regression.
4. As linear regression not giving good result so implemented RandomForestRegressor.
5. Later by usign RandomSearchCV used to tune the parameter and come up with **RMSE:1150**
6. Tried by using Xgboost Regressor but not able to reduce RMSE.
7. In future will try another algorithms and tune it so RMSE can get reduce more.


# 2. Identify the Sentiments

Sentiment analysis remains one of the key problems that has seen extensive application of natural language processing. This time around, given the tweets from customers about various tech firms who manufacture and sell mobiles, computers, laptops, etc, the task is to identify if the tweets have a negative sentiment towards such companies or products.

**Evaluation Metric :**
The metric used for evaluating the performance of classification model would be weighted F1-Score.

[Please checkout the notebook for the result and approch](https://github.com/Pravin1Borate/Hackathon/blob/main/sentimental_analysis/Sentimental_analysis.ipynb)

For the above hackthon total **6910** people current rank for is **291**

### Approch:
**Data Processing: **
1. Lower-case all characters
2. Remove twitter handles
3. Remove urls
4. Replace unidecode characters
5. Only keep characters
6. Keep words with length>1 only
7. Replace words like 'whatisthis' to ' what is this'
8. Remove repeated spaces

**Result of classification:** \
![alt text](https://github.com/Pravin1Borate/Hackathon/blob/main/sentimental_analysis/images/confusionmatrixreport.png "Logo Title Text 1")
