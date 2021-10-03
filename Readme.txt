Introduction
Life expectancy is a statistical measure of a typical period a human being is expected to live. In the past, there have been numerous studies commenced on factors affecting life expectancy depending on various factors like demographic variables, income composition and mortality rates. It was uncovered that the effect of immunizations and the human development index was not considered in the past. The data for this project is collected from “The World Health Organization” & “United Nations website” from the period of 2000 to 2016 for 183 countries. The project relies on the accuracy of the data and will emphasize immunization factors, mortality factors, economic factors, social factors, and other health related factors. For every country, it’s much easier to find the predicting factor which is weighted lower in the value of life expectancy because factors in the dataset are built on different countries. This will help countries come up with an appropriate plan to improve the overall life expectancy of a given population.


Research Question
The main motivation for this project is predicting a country’s life expectancy. Our primary objective is to understand how immunizations, health, social and economic variables could affect this number.
This type of information should allow governments to establish policies, regulations, and laws that could potentially enhance communities’ well-being.


Relevant Domain
Life Expectancy rate of the country considering various factors.
https://www.kaggle.com/mmattson/who-national-life-expectancy?select=who_life_exp.csv
https://ourworldindata.org/life-expectancy
https://population.un.org/wpp/Download/Standard/Mortality/


Handling Null Values
Some features have more than 20% of missing values. We will not use these in the models.
For others, we will replace/fill in with the meaning of the country.
The list of columns that needs to be removed (have more than 20% of missing values) -
hospitals
hepatitis
doctors
gni_capita
une_hiv
une_poverty
une_edu_spend
une_literacy
Une_school


Conclusion
Unique about data : Time series
Imbalances : Nulls, Outliers, Skewness
Problems Faced: Messy data (outliers, null values, skewness) and continuous nature of features.
Resolving the issues :  Non-normalized data handling, using substituting Country-group mean, imputing the null values, winsoring, scalar and log transformation.
Creating additional features/variables: Modified the predictor feature-life expectancy which is continuous in nature & Created Life-expectancy class/groups to fit the classier model.
Models: Logistic Regression, Decision Tree, Random Forest
Evaluation : RSME, test set scores & model accuracy, classification report recall, precision & accuracy.
Best Results: Random Forest with 0.97 accuracy.