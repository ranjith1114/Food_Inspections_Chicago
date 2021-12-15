# Food Inspection : City of Chicago

### Problem Overview
- As a foodie, I'm constantly interested in trying new restaurants. As a result, in this project, I opted to fulfill my cravings by gathering and analyzing data from food outlets.   
- Based on data from the Chicago Data Portal, an analysis of food inspection was conducted. These inspections promote public health in areas of food safety and prevent the occurrence of foodborne illness.  
- The project's goal is to investigate restaurants in Chicago, based on the inspection type and Violations we should classify whether the Results is pass, pass with conditions or fail.  
- It is multiple classification problem.  
- Here violations is a feature variable and Results column is target variable.  

### Data description
- Chicago food inspection dataset contains information from inspections of restaurants and other food establishments in Chicago from January 1, 2010 to the present.
- It consist of 228330 rows and 17 columns.  
- Data : https://data.cityofchicago.org/api/assets/BAD5301B-681A-4202-9D25-51B2CAE672FF
- Dataset : https://data.cityofchicago.org/Health-Human-Services/Food-Inspections/4ijn-s7e5/data

# Exploratory Data Analysis.
- Only the violations column consist more missing values.
- As it is a huge dataset we can drop all the Nan values.
- If we impute the violation column also it's not useful for better analysis as it consist of text data.
- We have a huge amount of data for better analysis I am considering only the inspection type with Canvass.
# Feature Selection.
- I have considered only violations column for predicting the target variable.

# Findings
- Performance of Random Forest is good with 91% accuracy.  
- Followed by Decision tree model is good with 90% accuracy.  
- Logistic Regression performance is very low.  

# Further Exploration
- The purpose is to improve the food produced in the Chicago area in terms of quality, health, and efficiency. We want to improve our data analysis by developing a prediction model that combines environmental data to assist us target and correct food inspection violations at their sources.  

- In further, we can fine-tune hyperparameters, add meteorological data, and provide inspectors with the shortest way between sites, allowing them to save time and money by visiting many locations.

# References
- https://data.cityofchicago.org/Health-Human-Services/Food-Inspections/4ijn-s7e5/data
- https://data.cityofchicago.org/api/assets/BAD5301B-681A-4202-9D25-51B2CAE672FF
- https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html
- https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html
- https://scikit-learn.org/stable/modules/generated/sklearn.tree.DecisionTreeClassifier.html
- https://www.kaggle.com/hamditarek/food-inspections-in-chicago-eda-and-modeling#Show-suspected-locations-in-the-map-with-Risks-High-and-Medium
