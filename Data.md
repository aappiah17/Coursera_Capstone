
## Data 
The data to be used for this analysis comes from Kaggle.com (https://www.kaggle.com/tsiaras/uk-road-safety-accidents-and-vehicles). The original data is from the UK’s Department for Transport. There are two data sources available:
* Accident information, which contains information on distinct traffic accidents from 2005 to 2017. This dataset contains attributes, include a target variable for accident severity, that can be used in machine learning models. This dataset contains 2,047,256 rows and 34 columns.
* Vehicle information, which contains information on the vehicles involved in the accident and passenger information from 2004 to 2016. This dataset contains 2,177,205 rows and 24 columns. 
 
 
 
*Features for modelling*

The two datasets can be joined together using a distinct ID (Accident_Index). I will join them into one dataset and then select the features to be used for modelling. The target variable will be Accident_Severity. Features for training the model will include the following: 
 * Day_of_Week
 * Junction_Detail
 * Light_Conditions
 * Road_Type
 * Speed-Limit
 * Urna_or_Rural_Area
 * Weather_Conditions
 * Age_of_Vehicle
 * Engine_Capacity
 * Sex_of_Driver
 * Age_of_Driver
 * Was_Vehicle_Left_Hand_Drive
 * Vehicle_Type
 
*Exploring the target variable*

The distribution of the target variable shows that the data is highly unbalanced, with the vast majority of accidents (85%) categorized as slightly severe. That poses issues for modelling and therefore will be addressed appropriately. In addition, given how small the proportion of fatal cases are, it will be grouped together with the serious category, making this a binary classification problem. 
 
*Additional data preprocessing* 

Other data preprocessing steps that will be conducted includes standardizing all numeric variables, one hot encoding of all categorical variables, identifying appropriate methods for dealing with missing data. 
The data from 2005 to 2014 will be used to train the machine learning classification models and then the models will be tested using the data from 2015 to 2017. 




```python

```
