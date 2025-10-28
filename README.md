# Flight Fare Prediction

The business case of the Flight Fare Data set was to build a machine learning model to help predict the fare of various airlines in the future and let people decide and plan their travel. The data set has 10 features like Airline, Destination, Source, Departure time, Arrival time etc. The data set has a target column (output) as Price of the tickets purchased by the passengers who travelled earlier. Based on these previous records, the we had to build a model which could predict the future prices of the tickets and help travelers choose the best priced Airline for their future trips which could be cheaper for them.

To make predictions based on the available data set, different Machine Learning Algorithms were build as mentioned below:

Linear Regression
Support Vector Machine
K-Nearest Neighbour
Decision Tree
Random Forest
XGBoost
Gradient Boosting
Out of all models above, Random Forest Algorithm, XGBoost Algorithm and Gradient Boosting Algorithm performed best with a R2 score of 0.87, 0.85 and 0.83 respectively. After Hyperparameter Tuning, all these algorithms gave an improved R2 score of 0.89.

In other words, it can be said that 89% of the data are fitting correctly into the model.

**Report on Challenges Faced**
Missing Values: There were very less missing data in the data set in Route and Total_Stops columns. These null values were dropped as such less missing data will not impact the data set

**Date Formatting**: The "Date_of_Journey" column was not in a standard date format and this was challenging in performing the date based analyses. Hence, we used the below mentioned technique to handled these data:

Date Parsing: The "Date_of_Journey" column was converted to a standardized date format (e.g., YYYY-MM-DD) to facilitate date-based calculations and comparisons. This was done by splitting the date string, extracting day, month, and year and then reformatting was done.
Duration Data: The "Duration" column contained values in a non-standard format (e.g., "2h 50m"). Extracting meaningful insights from this column required converting it into a numeric format. The Technique used here is as follows:

Duration Conversion: The "Duration" column was transformed into a numeric format, representing the total duration of the journey in minutes. This involved splitting the string, extracting hours and minutes and converting them into minutes for easy analysis.
Categorical Data: There were several columns like "Airline," "Source," "Destination," and "Total_Stops," that were categorical in nature. Theses columns were handled using Label Encoder and converted to Numerical Data type.

Conclusion
Using Flight Fare Prediction Dataset, I analyzed various data provided using different exploratory data analysis methods with the help of seaborn and matplotlip libraries. This data set is a supervised learning dataset so we used various regression models to do some predictions about the price of the flight based on some features like type of airline, what is the arrival time, what is the departure time, what is the duration of the flight, source, destination etc.

It can be concluded that among various models applied to this dataset, Random Forest Algorithm, XGBoost Algorithm and Gradient Boosting Algorithm performed best. The R2 score for all three algorithms were 0.89 which means that almost 89% of the data fit perfectly into the model and hence do the correct prediction.
