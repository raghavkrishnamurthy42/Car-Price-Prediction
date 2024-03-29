# Car Price Prediction

# Note: The coding part of the project was equally shared and contributed by all the 3 team members stated below

- [ ] Venkataraman B (20BCE1499)
- [ ] Rohit Madhavan S (20BCE1150)
- [ ] Raghav K (20BCE1468)

This can also be seen in the right hand side of the main section --> Contributors

# Objective and Problem Statement

The main aim of this project is to predict the price of used cars using the various Machine Learning (ML) models. This can enable the customers to make decisions baesd on different inputs or factors namely 

- [ ] Brand or Type of the car one prefers like Ford, Hyundai etc
- [ ] Model of the car namely Ford Figo, Hyundai Creta
- [ ] Location like Delhi, Chennai, Mumbai
- [ ] Year of manufacturing like 2020, 2021 etc
- [ ] Type of fuel namely Petrol, Diesel
- [ ] Price range or Budget
- [ ] Type of transmission which the customer prefers like Automatic or Manual 
- [ ] Mileage 

to name a few characterisitic features required by the customer. The project Car Price Prediction deals with providing the solution to these problems. Through this project, we will get to know which of the factors are significant and tell us how they affect the car's worth in the market

# Dataset

https://www.kaggle.com/austinreese/craigslist-carstrucks-data

# Details about the dataset

The dataset has 26 columns which has details of 

- [ ] Unique ID, where no two cars can have same ID
- [ ] Region where the car is available 
- [ ] Price of the car which also includes the price range
- [ ] Year of manufacture like 2020, 2021 etc
- [ ] Brand or Type of the car
- [ ] Name of the manufacturer
- [ ] Model of the car

to name a few. These are the primary needs the customer looks into before buying a second hand car. We can also add some additional features that can enhance the chances of the customer and also helps in the sales of the cars

The image attached below shows the reference of the details that are contained in the dataset

![image](https://user-images.githubusercontent.com/73659436/157170886-bdc786a6-2c75-4180-bb39-8682ed87c158.png)

# Model used 
Multiple linear regression model is used which is characterized by more than 1 independent variables. 
# Tasks to perform on the dataset

The tasks that are to be done in this project are divided into various categories namely

# Data exploration and understanding

![image](https://user-images.githubusercontent.com/73659436/157187541-f89e5bbd-0efd-4a9d-b18c-30b4ea243212.png)

The image shown above describes us that the dataset has 205 rows and 26 columns. All the columns except Price are independent factors or variables. We again subdivide independent variables as Categorical and Numerical Variables

Some of the Numerical variables include

- [ ] wheelbase
- [ ] carlength
- [ ] carwidth
- [ ] carheight
- [ ] curbweight
- [ ] enginesize
- [ ] boreratio’, ‘stroke
- [ ] compressionratio
- [ ] horsepower
- [ ] peakrpm
- [ ] citympg
- [ ] highwaympg

Some of the Categorical variables include

- [ ] symboling
- [ ] fueltype
- [ ] aspiration
- [ ] doornumber
- [ ] carbody
- [ ] drivewheel
- [ ] enginelocation
- [ ] enginetype
- [ ] cylindernumber
- [ ] fuelsystem
- [ ] car_name



# Data Cleaning

There are no missing values in the dataset and also all the columns in the dataset are in the correct format except for Symboling which is a Categorical value. Also Data Preprocessing has been done on CarName and have created a new factor or variable instead of former and called it car_company

# Data Preparation

- [ ] Firstly, we need to prepare data for building the model, which requires us to split the data into X and Y as shown in the figure
- [ ] Secondly, create dummy variables for the independent variables
- [ ] Split the dataset into train and test 
- [ ] Model Building involves building the model with all necessary features using Linear Regression. We find out that the value as r-squared as 83% 
- [ ] Decide and choose the features for building the model. One such way for choosing the features is to plot no of features in the model to the value of r-squared
 as shown in the figure below

![image](https://user-images.githubusercontent.com/73659436/157192299-d0bf865d-fa58-4475-9580-5af4c6696e52.png)

# Building the suitable model and evaluating it

After deciding upon the data preparation, we finally come to the model building part wherein the final model is built using 6 different features as shown in the figure and we get the value of r2-squared to be 0.8851 which tends the model to have accuracy of 88.51%

![image](https://user-images.githubusercontent.com/73659436/157193097-3a862dcc-1086-4c08-8a2b-e60ae64b61ab.png)

# Evaluating the final model

In the model, we must ensure to test that the error terms are always normally distributed having mean equal to zero, with less correlation with the predictors and lastly, the variance of the error terms must be constant. We then plot the error terms. Thus, we come to know that the conclusion that final predictors have high value of correlation

![image](https://user-images.githubusercontent.com/73659436/157193794-479fa8bf-ca4b-40fe-8d5b-27d40b2b3a0f.png)
