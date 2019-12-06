# Data-Analysis-Vehicles
Data Analysis on various parameters of vehicles to predict the which attributes determine price of vehicle

<h2>Steps</h2>
<ul>
<li>Data Collection</li>
<li>Data Wrangling</li>
<li>Exploratory Data Analysis</li>
<li>Model Development</li>
<li>Model Evaluation and refinement</li>
</ul>

<h2>Data Collection </h2>

Dataset from:
<a href='https://s3-api.us-geo.objectstorage.softlayer.net/cf-courses-data/CognitiveClass/DA0101EN/module_5_auto.csv'>https://s3-api.us-geo.objectstorage.softlayer.csv </a>


<h2>Data Wrangling</h2> 
It invovles data cleaning and transforming into proper format

Exploratory data analysis
After finding the positive linear relations, concluded that <b>Engine size and highway mpg</b> are good predicator ofor price of car. 
Whereas <b>Peak rpm</b> does not seem like a good predictor of the price 

The categorical variables can have the type "object" or "int64". A good way to visualize categorical variables is by using boxplots
<b>Engine-location and drive-wheels</b> can be a good predicator whereas <b>body-style</b> attribute is not good

Value-counts is a good way of understanding how many units of each characteristic/variable we have
Applied on drive-wheels 
<p>We now have a better idea of what our data looks like and which variables are important to take into account when predicting the car price. We have narrowed it down to the following variables:</p>
Continuous numerical variables:
<ul>
    <li>Length</li>
    <li>Width</li>
    <li>Curb-weight</li>
    <li>Engine-size</li>
    <li>Horsepower</li>
    <li>City-mpg</li>
    <li>Highway-mpg</li>
    <li>Wheel-base</li>
    <li>Bore</li>
</ul>
    
Categorical variables:
<ul>
    <li>Drive-wheels</li>
</ul>

<p>As we now move into building machine learning models to automate our analysis, feeding the model with variables that meaningfully affect our target variable will improve our model's prediction performance.</p>

<h2>Model Development</h2>
Developing several models that will predict the price of the car using the variables or features. This is just an estimate but should give us an objective idea of how much the car should cost.

<p>Data Analytics, we often use <b>Model Development</b> to help us predict future observations from the data we have.</p>
<p>A Model will help us understand the exact relationship between different variables and how these variables are used to predict the result.</p>

<p>Comparing the three models(simple linear regression,multiple regression, polynomial), we conclude that <b>the MLR model is the best model</b> to be able to predict price from our dataset. This result makes sense, since we have 27 variables in total, and we know that more than one of those variables are potential predictors of the final car price.</p>

<h2>Model evaluation and Refinement</h2>
<p>After building models and making predictions of vehicle prices. This determine how accurate these predictions are.</p>
<p>Training and testing data</p>
<p>Checking cross validation score</p>
<p>Overfitting as It turns out that the test data sometimes referred to as the out of sample data is a much better measure of how well your model performs in the real world. </p>
<p>The distribution of the training is much better at fitting the data as compared to test data</p>
<p>Ridge Regression to see how the parameter Alfa changes the model.</p>
