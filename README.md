# Housing Price Prediction

This is a famous Kaggle problem where I  will implement various Machine Learning Models to predict "Sale Price" of houses.

The dataset used for modelling the problem statement is Armes Housing Dataset which is an alternative to commonly used Boston Housing dataset.

The work is implemented on Jupyter notebook in Python programming language.

## Description of Dataset

This housing dataset contains 80 variables, Among them, 57 are categorical variables and 23 are numerical variables.

###train.csv :
This file contains 1460 rows.

###test.csv:
This file contains 1459 rows.

###Xtrain.csv:
This file contains scaled features for training.

### Description of variables is as follows: 

SalePrice - the property's sale price in dollars. This is the target variable that you're trying to predict. MSSubClass: The building class MSZoning: The general zoning classification LotFrontage: Linear feet of street connected to property LotArea: Lot size in square feet Street: Type of road access Alley: Type of alley access LotShape: General shape of property LandContour: Flatness of the property Utilities: Type of utilities available LotConfig: Lot configuration LandSlope: Slope of property Neighborhood: Physical locations within Ames city limits Condition1: Proximity to main road or railroad Condition2: Proximity to main road or railroad (if a second is present) BldgType: Type of dwelling HouseStyle: Style of dwelling OverallQual: Overall material and finish quality OverallCond: Overall condition rating YearBuilt: Original construction date YearRemodAdd: Remodel date RoofStyle: Type of roof RoofMatl: Roof material Exterior1st: Exterior covering on house Exterior2nd: Exterior covering on house (if more than one material) MasVnrType: Masonry veneer type MasVnrArea: Masonry veneer area in square feet ExterQual: Exterior material quality ExterCond: Present condition of the material on the exterior Foundation: Type of foundation BsmtQual: Height of the basement BsmtCond: General condition of the basement BsmtExposure: Walkout or garden level basement walls BsmtFinType1: Quality of basement finished area BsmtFinSF1: Type 1 finished square feet BsmtFinType2: Quality of second finished area (if present) BsmtFinSF2: Type 2 finished square feet BsmtUnfSF: Unfinished square feet of basement area TotalBsmtSF: Total square feet of basement area Heating: Type of heating HeatingQC: Heating quality and condition CentralAir: Central air conditioning Electrical: Electrical system 1stFlrSF: First Floor square feet 2ndFlrSF: Second floor square feet LowQualFinSF: Low quality finished square feet (all floors) GrLivArea: Above grade (ground) living area square feet BsmtFullBath: Basement full bathrooms BsmtHalfBath: Basement half bathrooms FullBath: Full bathrooms above grade HalfBath: Half baths above grade Bedroom: Number of bedrooms above basement level Kitchen: Number of kitchens KitchenQual: Kitchen quality TotRmsAbvGrd: Total rooms above grade (does not include bathrooms) Functional: Home functionality rating Fireplaces: Number of fireplaces FireplaceQu: Fireplace quality GarageType: Garage location GarageYrBlt: Year garage was built GarageFinish: Interior finish of the garage GarageCars: Size of garage in car capacity GarageArea: Size of garage in square feet GarageQual: Garage quality GarageCond: Garage condition PavedDrive: Paved driveway WoodDeckSF: Wood deck area in square feet OpenPorchSF: Open porch area in square feet EnclosedPorch: Enclosed porch area in square feet 3SsnPorch: Three season porch area in square feet ScreenPorch: Screen porch area in square feet PoolArea: Pool area in square feet PoolQC: Pool quality Fence: Fence quality MiscFeature: Miscellaneous feature not covered in other categories MiscVal: $Value of miscellaneous feature MoSold: Month Sold YrSold: Year Sold SaleType: Type of sale SaleCondition: Condition of sale

## This implmentation involves following steps:
    
### 1. Exploratory Data Anaysis: 
         
Initially, data exploration step is performed which involves loading of training data, investigating missing values, outliers , number of numerical and categorical data, null values and relationship of different variables with target variable.

### 2. Feature Engineering:

Next, based on EDA, missing values are handled , categorical variables are encoded and necessary null columns are imputed on training and testing data.
          
### 3. Feature Scaling and Selection :

Since, the columns in the dataset contains values in different measuring units, therefore, min max scaler technique is used. Further, as the distribution is skewed, log transformation is used for converting the desired columns into gaussian distribution. Lasso Mpdel is used for selecting important variables that contributes in the final prediction.

### 4. Model implementation:

Various models are implemented such as Linear Regression, SVM  and ensemble techniques such as Random Forest.

## Result 

SVM model shows the best performance amongst the implemented models. R2_score metric is used for evaluating various machine learning models.
The SVM model  exhibits a R2_score of 88.43% without hyper-parameter tuning.

   
