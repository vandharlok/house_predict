
<h1>House Price Prediction Project</h1>
<h4>The dataset used in this project was obtained in KAGGLE</h4>

<h2>This project is all about predicting house prices using a bunch of different features like location, income, and the number of rooms. We did some data exploration, created new features, trained some models, and checked out how well they work.</h2>

<h3><strong>The Dataset</strong></h3>
<p>The data used is explained below:</p>
<ul>
    <li><strong>Longitude</strong>: How far west the house is. Higher numbers mean it's more to the west.</li>
    <li><strong>Latitude</strong>: How far north the house is. Higher numbers mean it's more to the north.</li>
    <li><strong>Housing Median Age</strong>: The average age of houses in a block. Lower numbers mean newer houses.</li>
    <li><strong>Total Rooms</strong>: Total number of rooms in a block.</li>
    <li><strong>Total Bedrooms</strong>: Total number of bedrooms in a block.</li>
    <li><strong>Population</strong>: Number of people living in a block.</li>
    <li><strong>Households</strong>: Number of households (groups of people living together) in a block.</li>
    <li><strong>Median Income</strong>: Average income for households in a block (in tens of thousands of USD).</li>
    <li><strong>Median House Value</strong>: Average house value in a block (in USD).</li>
    <li><strong>Ocean Proximity</strong>: How close the house is to the ocean.</li>
</ul>

<h3><strong>Making New Features</strong></h3>
<p>We came up with some new features to help our models do better:</p>
<ul>
    <li><strong>Bedroom Ratio</strong>: The ratio of total bedrooms to total rooms. This helps us see how many bedrooms there are compared to all the rooms.</li>
    <li><strong>Household Rooms</strong>: Average number of rooms per household. This shows how much living space there is per household.</li>
    <li><strong>Ocean Proximity Encoding</strong>: Turned the 'oceanProximity' feature into numbers using one-hot encoding, so our models can use it properly.</li>
</ul>

<h3><strong>Separating the data into test and train</strong></h3>
<p>We split the data into training and testing sets. This helps us make sure our model works well on new, unseen data.</p>

<h3><strong>Training the Models</strong></h3>

<h4>Linear Regression</h4>
<p>We trained a Linear Regression model and checked how it did using:</p>
<ul>
    <li><strong>R2 Score</strong>: Tells us how much of the variation in house prices our model explains.</li>
    <li><strong>RMSE (Root Mean Squared Error)</strong>: Tells us how far off our predictions are, on average.</li>
</ul>

<h4>Random Forest</h4>
<p>We also tried a Random Forest model.</p>

<h4>Hyperparameter Tuning</h4>
<p>We tweaked the settings of the Random Forest model to make it work even better, but was not the case</p>

<h3><strong>Checking How We Did</strong></h3>
<p>We looked at:</p>
<ul>
    <li><strong>R2 Score</strong></li>
    <li><strong>RMSE (Root Mean Squared Error)</strong></li>
</ul>
<p>These metrics helped us see how accurate our models were and how much error there was in our predictions.</p>

<p>Results that we obtain:</p>
<ul>
    <li><strong>R2 Score using Linear Progression: 0.6731</strong></li>
    <li><strong>RMSE using Linear Progression:66530.45
</strong></li>
</ul>
<ul>
    <li><strong>R2 Score using Random Forest  0.81285</strong></li>
    <li><strong>RMSE using Random Forest :50058.15
</strong></li>
</ul>
<h5>As we can see from the performances, using random forest the model was much better</h5>

