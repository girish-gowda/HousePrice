# HousePrice

imported libraries numpy, pandas, matplotlib.pyplot, seaborn, pandas.api.types.is_numeric_dtype and keras.utils.to_categorical

#HousePrice Dataset download link https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data

#Droped columns "Alley", "PoolQC", "MiscFeature" containing more missing values

#Droped the column "Id", which is of no use in prediction

#Column accepting only numeric values, replace the empty cells with mean of values #Column accepting only categorical values, replace the empty cells with mode of values

Now the Data is ready to use for Model Creation using XGBRegressor and RandomForestRegressor with estimators = 500

I have tried for best possible fit using cleaned data with below algorithms:

xgboost.XGBRegressor()
from sklearn.ensemble import RandomForestRegressor

RandomForestClassifier has providing 98.13% accuracy rate and submitted on kaggle competition

Model is saved using pickle library with ['Id', 'SalePrice'] columns

This code in kaggle competition rank is 3316/5542
