# Common Techniques for House Price Prediction:

1. Linear Regression

   - Basic but effective for price relationships with features
   - Easy to interpret results
   - Assumes linear relationship between variables

2. Random Forest

   - Handles non-linear relationships
   - Good with numerical and categorical features
   - Less prone to overfitting
   - Can handle missing values

3. XGBoost/LightGBM
   - Advanced gradient boosting algorithms
   - Usually provides better accuracy
   - Good for large datasets
   - Handles various feature types

Key Features to Consider:

- Location (neighborhood, zip code)
- Square footage
- Number of bedrooms/bathrooms
- Year built
- Property type
- Crime rate
- School ratings
- Distance to amenities
- Public transportation access

Steps:

1. Data cleaning and preprocessing
2. Feature engineering
3. Model selection and training
4. Cross-validation
5. Hyperparameter tuning
6. Model evaluation using metrics like RMSE, MAE

## Papers

### Housing prediction via improved machine learning

https://www.sciencedirect.com/science/article/pii/S1877050920316318

#### Preprocessing

• Remove attributes indicating the number of kitchens, bathrooms, and drawing rooms due to their ambiguity.
• Set the number of living rooms (bedrooms were mistranslated to living rooms) in a range from 1 to 4.
• Add attribute “distance” indicating the distance of the house from the center of Beijing.
• Replace attribute “constructionTime” with attribute “age” by deducting the year that the house constructed from
the current year (2019).
• Set minimum values for attributes “price” and “area”.
• Split the attribute “floor” into attributes “floorType” and “floorHeight”.
• Take outliers into consideration.

#### Descriptiva

We could see different correlations: District vs Price, Building type vs Price, Building type vs Area

#### Errors

RMSE

#### ML techinques used in the paper

RandomForestClassifier
Extreme Gradient Boosting (XGBoost) -> Tree boosting  
Best technique was Stacked generalization, which consisted of Randome Forest first and then XGBoost

###House price prediction using machine learning
https://www.irjet.net/archives/V11/i4/IRJET-V11I4226.pdf

Conclusion is basically the same, Random forest + Gradient boosting seems to work best.

###Predicting housing prices and analyzing real estate market in the Chicago suburbs using Machine Learning
https://arxiv.org/abs/2210.06261

Seems that XGBoost is the best

###Predicting Rental Price of Lane Houses in Shanghai with Machine Learning Methods and Large Language Models
They also say that RF works bets.
Use MSE, MAE, R2 for error

Do the preprocessing and also,
Add a new variable called ”total-ssvalue” to facilitate subsequent modeling. (This variable represents the cumulative count of various soft furnishing facilities such as air conditioning, heating, and other amenities.)

# Conclusions about models

Main used error function is RMSE (last one uses MSE), MAE and R-square Score.
XGBoost or/and Random Forest for prediction seems to be the best.
State of the art with 10-shot seems to perform even better for shangai prices.
