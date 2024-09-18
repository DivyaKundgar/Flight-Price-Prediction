## Flight-Price-Prediction

# Files
- notebook.ipynb: Jupyter Notebook containing the code and analysis for the project.
- data.xlsx: Excel file containing the dataset used in the analysis.
  
# Dependencies
- Python 3
- Jupyter Notebook
- Libraries: numpy, pandas, seaborn, matplotlib

# What we will see in this Notebook
- Problem Statement
- Importing Libraries
- Loading the dataset
- Data Inspection
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Checking for null values
- Using Encoding to Handle categorical data
- Feature Selection
- Building Machine Learning models
- Hyperparameter Tuning
- Conclusion

### Problem Statement
I have build an ML model that predicts flight ticket prices based on various independent features, using a dataset of flight ticket prices. The dataset includes prices for various airlines and cities. The prediction results can be beneficial for both travelers, who can use it to make informed decisions about their travel, and for airlines, who can use it to forecast competitors' rates and adjust their pricing strategies to maximize revenue while remaining competitive.

# Domain Analysis
*In the domain analysis for the Flight price prediction project, key columns such as 'Airline',
'Date_of_Journey','Source','Destination','Route','Total_Stops','Additional_Info','Price','Dep_Time', 
'Arrival_Time', 'Duration' and 'Price' play pivotal roles in shapping Flight Prediction Outcomes.*

*The dataset used in the project contains information about airline tickets,including:*

- *Airline:* So this column will have all the types of airlines like Indigo,Jet Airways,Air India,and many more.

- *Date_of_Journey:* This column will let us know about the date on which the passenger's journey will start.

- *Source:* This column holds the name of the place to where passengers journey will start.

- *Destination:* This column holds the name of the place to where passengers wanted to travel.

- *Route:* He we can know about that what is the route through which passengers have opted to travel from his/her source to their destination.

- *Dep_Time:* This column holds the deparature time.

- *Arrival_Time:* Arrival time is when the passenger will reach his/her destination.

- *Duration:* Duration is the whole period that a flight will take to complete its journey from source to destination.

- *Total_Stops:* This will let us know in how many places flights will stop there for the flight in the whole journey.

- *Additinal_Info:* In this column, we will get information about food, kind of food, and other amenities.

Model	Accuracy
0	K-Nearest Neighbour	58.784150
1	Decision Tree	67.765084
2	Random Forest	80.138329

For Random Forest Regressor,
- Before hyper tuning, R2 score = 80 %
- After hyper tuning, R2 score = 82 % 
- The value of MAE drops as well, indicating that we are successful in tunning our model.

#Results
- The analysis includes exploratory data analysis, feature engineering, model trainning and evaluation. 
- For predicting the Price, we build 3 models using the following algorithms: 
  - K neighnors regressor
  - Decision Tree regressor
  - Random Forest Regressor
- Evaluation metrics: Mean Absolute Error, Mean squared Error, R2 Score

##### Conclusion

We have used random forest regressor for training the model and improved its accuracy by doing hyperparameter tuning. As a result, we have trained our **Random Forest Regression model**, to forecast fares of flight tickets, with an R2 score of 82 %.
