# STRIDE Project: Using historical vehicle transaction data to predict new vehicle sales

Jinpeng Gao
Transportation Technology and Policy

# Research question

The purpose of this project is to predict new car sales using historical vehicle transaction data in China vehicle market and determine the main driving factors for consumers to choose certain vehicles, therefore predicting energy use and greenhouse gas emissions.
My hypothesis is that for each vehicle make and model, the annual sales or seasonal sales are correlated with the characteristics of the vehicle model, including the vehicle price, purchase tax, type of fuel, curb weight, engine power, type of drivertrain, number of seats and doors and so on. Using these variables as independent variables, the probability of choosing one specific vehicle model will be calculated or the sales of one specific vehicle model will be calculated. My overarching question is how vehicle sales are impacted by vehicle characteristics listed in the data source section below. 

The first step: which characteristics are duplicated or highly correlated? This is what we are going to achieve during the incubator. 
The second step: which characteristics impact the vehicle sales and what's their relationships. This will be the question I will try to answer after the incubator. 

# Data source

I plan to collect data from *China Auto Market Almanac* and https://www.autohome.com.cn.
I plan to use 2010-2015 data as my training set and 2016 data as my validation set.

For each style of a certain vehicle model 
displacement, its characteristics could be divided into the following categories (need to be improved):
1) Basic information: the year when this vehicle was produced, vehicle manufacturers(dummy or categorical), vehicle type
(dummy or categorical, SUV, MPV, sedan, pick-up. etc)
2) Engine: cylinder, 
3) Powertrain: horsepower, transmission type, FF or FR, top speed, etc.
4) Fuel: efficiency, displacement, way of air intake, etc.
5) Dimension: LWH, wheelbase, #door, #seats
6) Safety equipment: ABS, radar,  airbag.
7) Exterior features: sunroof
8) Interior features: heated seats, GPS, bluetooth, TV, AC
9) Advanced technologies: autonomous vehicle technologies, park assist, drive assist
10) Alternative fuel vehicles: if not powered by gasoline.

Other important aggregate factors like GDP, disposable income, age may also be considered as generic variables. 
Provinces may also be considered as the dummy variables.

# Methodology

I will conduct a linear regression with the model sales as dependent variable and all other vehicle 
characteristics as the independent variables. I will also look at the correlation between variables and determine 
categorical or continuous variables. By feature engineering, I will determine the golden features that make consumers choose that cerntain vehicles.

Any file or script added to this repository will be added or linked out to storage location from one of the following components:
* Data management plan file (explains how data are to be organized, stored and shared)
* get_raw_data folder (scripts to get the data and a link to the storage of the directly downloaded data with no cleaning)
* analyze_data folder (scripts for any transformation of the raw data and links to the resulting processed dataset )
