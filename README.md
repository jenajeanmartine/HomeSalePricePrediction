# Home Sale Price Prediction - Ames, IA  |  Jena Brentano
​
​
## Problem Statement
The company, Zillow, needs to improve their predictive home sale price models in general, but here specifically for the city of Ames, Iowa or similar cities with huge growth potential. This will in turn positively affect their bottom line, as they maintain their leading position in the industry by providing reliable information to customers. These customers include prospective home buyers, sellers, real estate agents, and those in other related sectors. Zillow provides important information for prospective home buyers and sellers, and is a powerful platform for advertising or referrals for real-estate agents and service providers. Zillow is also expanding into the physical real estate market. What makes them an excellent resource to it's current customers can also enable a lucrative business model of flipping homes for a profit.
    
---
​
## Description of Data
Zillow has provided a dataset describing about 2050 homes with about 80 attributes which include qualitative and quantitative categories such as Overall Quality, Number of Rooms, Kitchen Quality, Garage Type, Misc. Feature Value, and of course, Sale Price.
    
### Data Dictionary
​
The data is available in detail here: http://jse.amstat.org/v19n3/decock/DataDocumentation.txt
​
## Primary Findings/Conclusions:
​
- Features that are most highly correlated to Sale Price in the given data are: Overall Quality, Ground Floor Living Area, Exterior Quality, Kitchen Quality, Garage Cars (# of cars).
​
- Because many of the provided home features are categorical/ordinal, it is important to convert these features using dummy variables or translating to numerical ratings in order to explore their potential uesfulness as predictors in a model.
​
- A powerful predictive model can be made with Linear Regression just by choosing features from the provided data with high correlations to Sale Price, but it's important to look at the statistical significance of these features on sale price to create a model that works well on new data. 
​
- Many of the 80 features in the dataset had little to no impact on the accuracy of the model. If it helps the bottom line to collect less data, Zillow has an opportunity to explore and tune which features are unecessary to record.
​
- Many feature categories are inter-related, and the features for a final predictive model should be carefully considered to avoid multi-collinearity, or inter-relatedness. This is to preserve the integrity of the model and to enable us to understand clearly the relationship of a specific feature to Sale Price. Creating many new interaction features automatically with Polynomial Features functions and using LASSO to select the most impactful features is an excellent method for creating a great predictive model, but requires careful scrutiny to avoid many potential cases of collinearity of model features
