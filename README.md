# Carbon-Footprint-Estimator
The Carbon Footprint Estimator is a regression-based machine learning project that predicts a person's weekly CO₂ emissions (in kilograms) based on their lifestyle choices—like diet, transportation, and electricity usage. It aims to:
1.Promote awareness about environmental impact
2.Help users understand how their choices contribute to carbon emissions
3.Suggest areas for lifestyle improvement

# Dataset Used
Link:https://www.kaggle.com/datasets/dumanmesut/individual-carbon-footprint-calculation
Features in dataset:
'Body Type': Body type.
'Sex': Gender.
'Diet': Diet.
'How Often Shower': Frequency of showering
'Heating Energy Source': Residential heating energy
'Transport': Transportation preference.
'Vehicle Type': Vehicle fuel type.
'Social Activity': Frequency of participating in social activities.
'Monthly Grocery Bill': Monthly amount spent on groceries, in dollars.
'Frequency of Traveling by Air': Frequency of using aircraft in the last month.
'Vehicle Monthly Distance Km': The kilometers traveled by vehicle in the last month.
'Waste Bag Size': Size of the garbage bag
'Waste Bag Weekly Count': The amount of garbage thrown away in the last week.
'How Long TV PC Daily Hour': Daily time spent in front of TV or PC.
'How Many New Clothes Monthly': Number of clothes purchased monthly.
'How Long Internet Daily Hour': Time spent on the Internet daily.
'Energy efficiency': Whether or not you care about purchasing energy efficient devices.
'Recycling': The wastes it recycles.
'Cooking_With': Devices used in cooking
'CarbonEmission': Dependent variable, total carbon emissions.


# Features & Flow
Exploratory Data Ananlysis:
1.Check for duplicates
2.Check for missing values
3.Check variables' types
4.Check the unique values
5.Use Label Encoding for categorical variables
6.Plot the correlation matrix as a heatmap with colors

   
# Model Training:
Model: A RandomForestRegressor was selected for its robustness and ability to handle mixed data types. 
Trained on input features to predict weekly CO₂ output
Out-of-Bag validation helps assess model performance on unseen data

Model Evaluation:
Mean Squared Error (MSE): Measures prediction error magnitude
R² Score: Indicates how much variance in carbon output is explained by the model
Out-of-Bag (OOB) Score: Internal accuracy metric using unused samples during bootstrapping

Visual output: 
Feature importance graph to show what affects predictions most

Output:
Predicted weekly CO₂ emissions (in kg)

# Dependencies
pandas – for data loading and preprocessing
numpy – for numerical operations
matplotlib & seaborn – for visualizing feature importance
scikit-learn – for model training, evaluation, and preprocessing (LabelEncoder, RandomForest, MSE, R²)

