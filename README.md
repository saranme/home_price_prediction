# Home price prediction
Prediction of the price of houses given their characteristics.

**Introduction**
* Each variable in the dataset describes the characteristics of the houses.
* The objective is to predict the price of the house given the independent variables.

**Index**
1. Variable description
2. Data Wrangling
3. Analysis of the target variable
4. Correlation and association
5. Variable normalization
6. Grouping and encoding of values
7. Concatenation of coded variables
8. Model RL
9. Model Errors
10. 10. Coeff. Determination
11. Model setting

1. Variable description
**SalePrice target variable**: house price.

**Meaning of continuous numerical variables**:
* *LotFrontage*: street feet belonging to the property.
* *LotArea*: Total area of the land property in square feet.
* *MasVnrArea* - Wall construction area in square feet.
* *BsmtFinSF1* - Type 1 basement finished area quality.
* *BsmtFinSF2*: quality of the second finished area (if any) of the type 2 basement.
* *BsmtUnfSF* - Square feet of unfinished basement area.
* *TotalBsmtSF* - Square footage of basement area.
* *1stFlrSF* - First floor square footage.
* *2ndFlrSF* - Second floor square footage.
* *GarageArea* - Square footage of the size of the garage.
* *WoodDeckSF* - Wood deck area in square feet.
* *GrLivArea* - Living area above ground in square feet.
* *OpenPorchSF* - Area of the open porch in square feet.
* *EnclosedPorch* - Area of the enclosed porch in square feet.
* *3SsnPorch* - Three station porch area in square feet.
* *ScreenPorch* - Screen porch area in square feet.
* *MiscVal* - Dollar value of miscellaneous features.
* *LowQualFinSF* - Square footage with low quality finish (all floors).
* *PoolArea* - Pool area in square feet
* *MiscVal*: Dollar value of miscellaneous attributes.
* *SalePrice*: price of the house.

**Meaning of discrete numerical variables**:
* *FullBath*: full baths above ground.
* *HalfBath*: half baths above ground.
* *BsmtFullBath* - Full baths in basement.
* *BsmtHalfBath* - Half full baths in basement.
* *BedroomAbvGr* - Above ground bedrooms (excludes basement bedrooms).
* *TotRmsAbvGrd* - Rooms above ground level (does not include bathrooms).
* *Fireplaces*: number of fireplaces.
* *GarageCars*: size of the garage in car capacity.
* *GarageYrBlt*: year of construction of the garage.
* *YearBuilt*: year of construction.
* *YearRemodAdd*: remodeling date (same as construction date if there are no remodels or additions).
* *YrSold*: year sold.
* *MoSold*: month sold.
* *KitchenAbvGr*: above-ground kitchens.

**Meaning of ordinal categorical variables**:
* *LotShape*: property shape (regular or irregular).
* *LandSlope:* pending property.
* *LandContour*: flatness of the property.
* *OverallQual*: note of the materials and finish of the house.
* *OverallCond*: note of the condition of the house in general.
* *ExterQual*: evaluates the quality of the exterior material.
* *ExterCond*: evaluates the current condition of the exterior material.
* *BsmtQual*: evaluates the height of the basement.
* *BsmtCond*: assesses the condition of the basement.
* *BsmtExposure*: refers to garden level walls.
* *HeatingQC*: heating quality and condition.
* *KitchenQual*: kitchen quality.
* *Functional*: functionality of the house.
* *FireplaceQu*: fireplace quality.
* *GarageFinish*: interior finish of the garage.
* *GarageQual*: garage quality.
* *GarageCond*: condition of the garage.
* *Utilities*: type of utilities available.
* *BsmtFinType1*: quality of finished basement area.
* *BsmtFinType2*: quality of the second finished area (if present).
* *CentralAir*: central air conditioning
* *PavedDrive*: paved driveway.

**Meaning of nominal categorical variables**:
* *MSZoning* - Identifies the general zoning classification of the sale.
* *LotConfig*: property configuration.
* *Neighborhood*: neighborhoods.
* *Condition1*: proximity to various conditions.
* *BldgType*: type of housing.
* *HouseStyle*: house style.
* *RoofStyle*: roof style.
* *Exterior1st*: exterior cladding of the house.
* *Exterior2nd*: exterior cladding of the house if there is more than one material.
* *MasVnrType*: masonry cladding type.
* *Foundation*: type of foundation.
* *Electrical*: electrical system.
* *GarageType*: type of garage.
* *SaleType*: type of sale.
* *SaleCondition*: condition of the sale.
* *MSSubClass*: the class of the building.
* *Street*: type of road access
* *Condition2*: proximity to the main road or rail (if a second is present).
* *RoofMatl*: roof material.
* *Heating*: type of heating.
