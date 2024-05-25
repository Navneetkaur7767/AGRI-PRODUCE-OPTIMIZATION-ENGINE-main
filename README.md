 # AGRI-PRODUCE OPTIMIZATION ENGINE


![App Screenshot](https://media.nationalgeographic.org/assets/photos/120/983/091a0e2f-b93d-481b-9a60-db520c87ec33.jpg)
## Build a predictive model so as to suggest the most suitable crops to grow based on the available climatic and soil conditions. 
## Some time Climatic Conditions are unpredictable such as due to sudden Rainfall or due to Frequent heat waves or because of Fluctuating humidity level cause Damage to the Farming 
## Due to which Farmer suffer a lot and they are not able to Utilize there Agricultural Land and its Potential Properly to  solve this problem we are using Precision Farming.
## Many factors affect the productivity of crops but two factors that affect crops productivity directly are,
## 1. Soil Conditions
## 2. Climate Conditions
## Keeping these factors in my mind, I tried to build a Machine Learning model that will take different Climate and Soil conditions and predict a crop that can make maximum growth in these certain conditions and I did. By using this model, agronomists will be able to know which crop is more productive.
# TOOLS AND SOFTWARE
## Python (including libraries like Pandas, matplotlib, etc.)
## Jupyter notebook
# DATASET
## I got the data Set from Kaggle to build such a model.
![App Screenshot](https://github.com/sukriti145/AGRI-PRODUCE-OPTIMIZATION-ENGINE/blob/screenshot/screenshot%20of%20dataset.jpeg?raw=true)

## N: Ratio of Nitrogen in the Soil
## P: Ratio of Phosphorous in the Soil
## K: Ratio of Potassium in the Soil
## Temperature: Temperature in Celsius
## Humidity: Relative Humidity in %
## PH: Ph value for the Soil
## Rain Fall: Rain Fall in 1mm
# Data Cleaning
## Data cleansing or data cleaning is the process of detecting and correcting (or removing) corrupt or inaccurate records from a record ## set, table, or database and refers to identifying incomplete, incorrect, inaccurate or irrelevant parts of the data and then coarse ## data or replacing, modifying, or deleting the dirty.There are no missing values and unwanted columns or rows.
![App Screenshot](https://github.com/sukriti145/AGRI-PRODUCE-OPTIMIZATION-ENGINE/blob/screenshot/Screenshot%202022-02-06%20at%2023-59-36%20Agricultural%20Production%20Optimization%20Engine%20-%20Jupyter%20Notebook.png?raw=true)
# PERFORMING EDA
## perform some Statistics to the parameter of given dataset so that we know the dataset well.In this we find the average of every      ## parameter in dataset.
![App Screenshot](https://github.com/sukriti145/AGRI-PRODUCE-OPTIMIZATION-ENGINE/blob/screenshot/Screenshot%20of%20EDA.png?raw=true)
## Then we find minimum value,maximum value and average of all parameter for each crop.
![App Screenshot](https://github.com/sukriti145/AGRI-PRODUCE-OPTIMIZATION-ENGINE/blob/screenshot/screenshot%20min,max,average%20of%20all%20parameter%20for%20each%20crop.jpeg?raw=true)
# DISTRIBUTION OF GRAPHS
![App Screenshot](https://github.com/sukriti145/AGRI-PRODUCE-OPTIMIZATION-ENGINE/blob/screenshot/screenshot%20of%20graph.png?raw=true)
## From the distribution graph, we can see that some crops require a small amount of Nitrogen, some require average, and some require ## large amounts. Some crops require a small amount of Phosphorous, some require average, and some require large amounts. Some crops ## ## require a small amount of Potassium, some require average, and some require large amounts. Some crops require low Temperature, some ## require average, and some require high. Some crops require low Humidity in soil, some require average, and some require high. Some ## crops require low PH levels and some require high PH levels. Some crops require low Rain Fall, some require average, and some      ## require high
# Machine Learning Model
## First of all, we drop the label column from our data set as we don't need this.
# Train-Test Split
## In machine learning models, the trained model should perform well on unseen data. To simulate the new, unseen data, the available data is subjected to data splitting whereby it is split into 2 parts (sometimes referred to as the train-test split). Particularly, the first part is the larger data subset that is used as the training set (such as accounting for 80% of the original data) and the second is normally a smaller subset and used as the testing set (the remaining 20% of the data). And it is not fixed to divide data into 80 ratios 20, you can split it in any way or based on certain conditions.
# Predictive Model
## Then, I import Logistic Regression from sklearn.linear_model, fit my model, and make a predictive model.
## Here, the code is not so complex but a question arises that why do we use Logistic Regression instead of Linear Regression?
## That is because when we have to deal with continuous variables or we can say with numerical values we use linear regression but when we have to deal with categorical variables we use logistic regression . Here we are dealing with categorical variables that's why we used logistic regression.
## logistic Regression is trying to map real values or independent data points in the interval from 0 to 1.
## Points below the cut off line belong to Class B and points above the cut off line belongs to class A
## Points in class A have the probability of a certain occurrence on the other hand points in class B have no probability of a certain occurrence.


