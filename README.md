## Project Overview

This project uses multiple linear regression modeling to analyze house sales in a northwestern county.

### Business Problem

The project consists in providing some key metrics to a real estate agency that helps homeowners buy and/or sell homes. The goal of the analysis is to determine what factors come into play when it comes to increasing the value of their home. 

### The Data

This project uses the King County House Sales dataset, which can be found in  `kc_house_data.csv` in the data folder in this assignment's GitHub repository. The description of the column names can be found in `column_names.md` in the same folder. The file used to perform the analysis contained 21,597 rows and 20 columns.

The target variable of the data set was the price. 

### Regression model

The analysis used linear regression. The model started intially with a simple linear regression and ended up evolving into a multivariable linear regression with 8 features.

### Results

[](Images/OLS_Regression_results.png)

### Conclusion

The purpose of the above analysis was to make a viable recommendation for real estate companies in order to help their homeowners clients sell their properties at best value.

The grade of a property is the highest factor that needs to be adressed: in order to increase the sale value: if we look at the grade coefficient, 0.1820, we can in fact read that for every 1 notch increase in the grade, the value of the property increases dy 18.2%.

There are several ways in which a property can be improved, depending on what would need to be done on the interior and/or exterior. For example, the homeowner can improve the quality of the AC/heating units, the plumbing pipes, the kitchen appliances, the flooring, the bathroom appliances, the alarm system, etc. Another detail that tends to increase the value of a home is to have it re-arranged by an interior designer.

For the exterior of the house, the outisde appearance of the property plays a very important role in the price component. Repainting the walls and re-cementing the front driveway for example can be considered as factors, such as re-doingthe roof or planting bushes.

When looking at the other coefficients, we can see that bedrooms and bathrooms are negative, which translates into the fact that it can negatively impact the price by 1.1% to 1.6% respectively of a home if only working on having nice bedrooms and bathrooms as opposed to the property. Some properties might be bigger but old, hence won't have a better grade than a smaller property that has a high grade.

The r-squared value, 0.582, indicates that the model can account for about 58% of the variability of price around its mean. The null hypothesis for multiple regression is that there is no relationship between the chosen explanatory variables and the response variable. Also, all of the p-values round to 0, which means we can reject the null hypothesis (except for bathrooms!). Now we can confirm that the model satisfies the assumptions of normality and homoscedasticity.

What could be the next steps?

Have a better understanding of what is taken into account when assessing the grade of a property. For example, does the property have a driveway, is it easy access for strollers/wheelchairs, or simply understand what components of the house matter the most to home buyers: new bathroom/kitchen appliances over fresh paint on the walls for example. Another factor that could help increase the sale of the property could be the choice of windows, whether they are double glazed or not.
Other factors that could help increase the value of a property that are harder to quantify such as the choices of plants/flowers/trees in the backyard, heated pool, outdoor shower...etc. All of these are factors that the property owner can improve.