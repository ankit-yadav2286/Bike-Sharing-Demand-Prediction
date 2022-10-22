# Bike-Sharing-Demand-Prediction

![image](https://user-images.githubusercontent.com/107911669/197341317-b4a7af0c-15d5-463a-bafb-ccde09f5cb56.png)

# Problem Statement
Currently Rental bikes are introduced in many urban cities for the enhancement of mobility comfort. It is important to make the rental bike available and accessible to the public at the right time as it lessens the waiting time. Eventually, providing the city with a stable supply of rental bikes becomes a major concern. The crucial part is the prediction of bike count required at each hour for the stable supply of rental bikes.

# Introduction

* Prediction of Bike Sharing demand can help bike sharing companies to allocate bikes better and ensure a more sufficient circulation of bikes for customers.
* This model proposes a real time method for predicting bike renting based on historical data,weather data and time data.
* This demand prediction model can provide a significant theortical basis for management strategies and vehicle scheduling in public bike rental system.

# Attribute Information:
### Date : year-month-day
### Rented Bike count - Count of bikes rented at each hour
### Hour - Hour of he day
### Temperature-Temperature in Celsius
### Humidity - %
### Windspeed - m/s
### Visibility - 10m
### Dew point temperature - Celsius
### Solar radiation - MJ/m2
### Rainfall - mm
### Snowfall - cm
### Seasons - Winter, Spring, Summer, Autumn
### Holiday - Holiday/No holiday
### Functional Day - NoFunc(Non Functional Hours), Fun(Functional hours)

# Data Pipeline
● Exploratory Data Analysis (EDA): In this part we have done some EDA on the features to see the trend.

● Data Processing: In this part we went through each attributes and encoded the categorical features.

● Model Creation: Finally in this part we created the various models. These various models are being analysed and we tried to study various models so as to get the best performing model for our project.

# Data Discovery

* The original dataset has 14 columns and 8760 rows
* Data types of various columns object,Float and Integer
* Dependent variable being Rented Bike Count and all other variables are our Independent variables

## Exploratory Data Analysis (EDA)

EDA refers to the critical process of performing initial investigations on data so as to discover patterns,to spot anamolies,to test hypothesis and to check assumptions with the help of summary statistics and graphical representations 

# Analysis of Data by Visualization
![image](https://user-images.githubusercontent.com/107911669/197342537-4f79fb09-8aad-4f31-8a64-43d8a2e3ef14.png)
![image](https://user-images.githubusercontent.com/107911669/197342558-92c48e03-5efb-4374-8393-b63c79c5cf9e.png)
![image](https://user-images.githubusercontent.com/107911669/197342567-622d384a-ba7e-447d-a53b-f198a829a83b.png)
![image](https://user-images.githubusercontent.com/107911669/197342586-144afa19-3a48-4124-8315-440073d91926.png)
![image](https://user-images.githubusercontent.com/107911669/197342599-4892e240-17f5-4e98-bbd6-4d90d8b5dc8f.png)
![image](https://user-images.githubusercontent.com/107911669/197342617-20267ea9-d26c-4b3b-a3d5-de3ade75550d.png)

# Hypothesis
* In summer season the use of rented bike is high whereas in winter season the use of rented bike is very low.
* The month 5 to 10 the demand of the rented bike is high as compare to other months.
* People generally use rented bikes during their working hour from 7am to 9am and 5pm to 8pm.
* in the week days which is in blue colur tells that the demand of the bike is higher because of the office as compare to the weekend.
* people use rented bike only in functioning day.
* use of rented bike is more on no holiday as compare to holiday.

# Visualizing Distributions
![image](https://user-images.githubusercontent.com/107911669/197342838-18578d65-24e5-4d8b-91b0-74b1082e03a5.png)

# Analysis from Distributions 
* "Temperature" and "Humidity" follows Uniform Distribution
* "Windspeed","Solar radition","Rainfall" and "Snowfall" are having right skewed distributions
* "Dew Point Temperature" and "Visibility" are having left skewed distributions.

# Distribution of Dependent Variable 
![image](https://user-images.githubusercontent.com/107911669/197343081-33dcc856-c6a7-491c-8fe8-b114c9bea072.png)
![image](https://user-images.githubusercontent.com/107911669/197343093-31d76857-2424-4c89-aea7-55b09086a7d0.png)

# Data Preprocessing and Assumption Check

![image](https://user-images.githubusercontent.com/107911669/197343258-6f2b1114-9560-4f9a-8326-550d70704436.png)

# Multicollinearity

![image](https://user-images.githubusercontent.com/107911669/197343282-16d68ff7-4c51-483d-86ad-9a9c476f525e.png)

there is a positive correlation between columns 'Temperature' and 'Dew point temperature' i.e 0.91 so even if we drop this column then it dont affect the outcome of our analysis

# Algorithms Used

Linear Regression
Lasso and Ridge Regression
Decision tree
Random Forest
Gradient Boosting

# Conclusions
● When we compare the root mean squared error and mean absolute error of all the models, the random forest regression model has less root mean squared error and mean absolute error, ending with the R-squared of 99% . So, finally this model is best for predicting the bike rental count on daily basis.

● For all the models, temperature or hour was ranked as the most influential variable to predict the rental bike demand at each hour.

# Challenges

* Feature Engineering 
* Feature Selection
* Model Training and Performance improvement
