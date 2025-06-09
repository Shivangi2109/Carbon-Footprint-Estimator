# Carbon-Footprint-Estimator
The Carbon Footprint Estimator is a regression-based machine learning project that predicts a person's weekly CO₂ emissions (in kilograms) based on their lifestyle choices—like diet, transportation, and electricity usage. It aims to:<br>
1.Promote awareness about environmental impact<br>
2.Help users understand how their choices contribute to carbon emissions<br>
3.Suggest areas for lifestyle improvement<br>

# Dataset Used<br>
Link:https://www.kaggle.com/datasets/dumanmesut/individual-carbon-footprint-calculation<br>
Features in dataset:<br>
'Body Type': Body type.<br>
'Sex': Gender.<br>
'Diet': Diet.<br>
'How Often Shower': Frequency of showering.<br>
'Heating Energy Source': Residential heating energy.<br>
'Transport': Transportation preference.<br>
'Vehicle Type': Vehicle fuel type.<br>
'Social Activity': Frequency of participating in social activities.<br>
'Monthly Grocery Bill': Monthly amount spent on groceries, in dollars.<br>
'Frequency of Traveling by Air': Frequency of using aircraft in the last month.<br>
'Vehicle Monthly Distance Km': The kilometers traveled by vehicle in the last month.<br>
'Waste Bag Size': Size of the garbage bag.<br>
'Waste Bag Weekly Count': The amount of garbage thrown away in the last week.<br>
'How Long TV PC Daily Hour': Daily time spent in front of TV or PC.<br>
'How Many New Clothes Monthly': Number of clothes purchased monthly.<br>
'How Long Internet Daily Hour': Time spent on the Internet daily.<br>
'Energy efficiency': Whether or not you care about purchasing energy efficient devices.<br>
'Recycling': The wastes it recycles.<br>
'Cooking_With': Devices used in cooking.<br>
'CarbonEmission': Dependent variable, total carbon emissions.<br>


# Features & Flow:<br>
Exploratory Data Ananlysis:<br>
1.Check for duplicates<br>
2.Check for missing values<br>
3.Check variables' types<br>
4.Check the unique values<br>
5.Use Label Encoding for categorical variables<br>
6.Plot the correlation matrix as a heatmap with colors<br>

   
# Model Training:<br>
Model: A RandomForestRegressor was selected for its robustness and ability to handle mixed data types.<br>
Trained on input features to predict weekly CO₂ output.<br>
Out-of-Bag validation helps assess model performance on unseen data.<br>

Model Evaluation:<br>
Mean Squared Error (MSE): Measures prediction error magnitude.<br>
R² Score: Indicates how much variance in carbon output is explained by the model.<br>
Out-of-Bag (OOB) Score: Internal accuracy metric using unused samples during bootstrapping.<br>

Visual output: <br>
Feature importance graph to show what affects predictions most.<br>

Output:<br>
Predicted weekly CO₂ emissions (in kg).<br>

# Dependencies<br>
pandas – for data loading and preprocessing.<br>
numpy – for numerical operations.<br>
matplotlib & seaborn – for visualizing feature importance.<br>
scikit-learn – for model training, evaluation, and preprocessing (LabelEncoder, RandomForest, MSE, R²).<br>

