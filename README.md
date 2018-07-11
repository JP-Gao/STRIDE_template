# STRIDE Project: Using historical vehicle transaction data to predict vehicle sales

Jinpeng Gao
Transportation Technology and Policy

# Research question

The purpose of this project is to predict vehicle sales using historical vehicle transaction data in China vehicle market.
My hypothesis is that for each vehicle make and model, the annual sales or seasonal sales are correlated with the characteristics of the vehicle model, including the vehicle price, purchase tax, type of fuel, curb weight, engine power, type of drivertrain, number of seats and doors and so on. Using these variables as independent variables, the probability of choosing one specific vehicle model will be calculated or the sales of one specific vehicle model will be calculated.

# Data source

I plan to collect data from *2004-2016 China Auto Market Almanac* and https://www.autohome.com.cn.
I plan to use 2004-2014 data as my training set and 2015~2016 data as my validation set.

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

# Methodology

I will conduct a basic linear regression first with the model sales as dependent variable and all other vehicle 
characteristics as the independent variables. I will also look at the correlation between varialbes and determine 
categorical or continuous variables.After the linear regression, I will also try different approaches like discrete
 choice model, random forest, support vector machine and so on.

Any file or script added to this repository will be added or linked out to storage location from one of the following components:
* Data management plan file (explains how data are to be organized, stored and shared)
* get_raw_data folder (scripts to get the data and a link to the storage of the directly downloaded data with no cleaning)
* analyze_data folder (scripts for any transformation of the raw data and links to the resulting processed dataset )
