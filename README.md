# Predicting the Sale Price of Bulldozers using Machine Learning
This is an end to end SalePrice prediction of Buldozers, based on Blue Book for Bulldozers dataset on Kaggle

<img src = "bulldozer-new.jpg">

**In this notebook, we're going to go through an example machine learning project with the goal of predicting the sale price of bulldozers.**

## 1. Problem definition

> How well we can predict the future sale price of a bulldozer, given its characteristics and previous examples of how much similar bulldozers have been sold for?

## 2. Data

The data is downloaded from  Kaggle Bluebook for Bulldozers competition!
https://www.kaggle.com/competitions/bluebook-for-bulldozers/data

Data is split into three parts:

* `Train.csv` is the training set, which contains data through the end of 2011.
* `Valid.csv` is the validation set, which contains data from January 1, 2012 - April 30, 2012 You make predictions on this set throughout the majority of the competition. Your score on this set is used to create the public leaderboard.
* `Test.csv` is the test set, which won't be released until the last week of the competition. It contains data from May 1, 2012 - November 2012.

## 3. Evaluation

The evaluation metric for this project is the RMSLE (root mean squared log error) between the actual and predicted auction prices.

https://www.kaggle.com/competitions/bluebook-for-bulldozers/overview/evaluation

**Note:** The goal for most regression evalution metrics is to minimize the error. For example, our goal for this project will be to build a machine learning model which minimizes RMSLE.

## 4. Features

The features can be seen below alog with their description:

		Variable	Description
0	SalesID	unique identifier of a particular sale of a machine at auction
1	MachineID	identifier for a particular machine; machines may have multiple sales
2	ModelID	identifier for a unique machine model (i.e. fiModelDesc)
3	datasource	source of the sale record; some sources are more diligent about reporting attributes of the machine than others. Note that a particular datasource may report on multiple auctioneerIDs.
4	auctioneerID	identifier of a particular auctioneer, i.e. company that sold the machine at auction. Not the same as datasource.
5	YearMade	year of manufacturer of the Machine
6	MachineHoursCurrentMeter	current usage of the machine in hours at time of sale (saledate); null or 0 means no hours have been reported for that sale
7	UsageBand	value (low, medium, high) calculated comparing this particular Machine-Sale hours to average usage for the fiBaseModel; e.g. 'Low' means this machine has less hours given it's lifespan relative to average of fiBaseModel.
8	Saledate	time of sale
9	Saleprice	cost of sale in USD
10	fiModelDesc	Description of a unique machine model (see ModelID); concatenation of fiBaseModel & fiSecondaryDesc & fiModelSeries & fiModelDescriptor
11	fiBaseModel	disaggregation of fiModelDesc
12	fiSecondaryDesc	disaggregation of fiModelDesc
13	fiModelSeries	disaggregation of fiModelDesc
14	fiModelDescriptor	disaggregation of fiModelDesc
15	ProductSize	The size class grouping for a product group. Subsets within product group.
16	ProductClassDesc	description of 2nd level hierarchical grouping (below ProductGroup) of fiModelDesc
17	State	US State in which sale occurred
18	ProductGroup	identifier for top-level hierarchical grouping of fiModelDesc
19	ProductGroupDesc	description of top-level hierarchical grouping of fiModelDesc
20	Drive_System	machine configuration; typcially describes whether 2 or 4 wheel drive
21	Enclosure	machine configuration - does machine have an enclosed cab or not
22	Forks	machine configuration - attachment used for lifting
23	Pad_Type	machine configuration - type of treads a crawler machine uses
24	Ride_Control	machine configuration - optional feature on loaders to make the ride smoother
25	Stick	machine configuration - type of control
26	Transmission	machine configuration - describes type of transmission; typically automatic or manual
27	Turbocharged	machine configuration - engine naturally aspirated or turbocharged
28	Blade_Extension	machine configuration - extension of standard blade
29	Blade_Width	machine configuration - width of blade
30	Enclosure_Type	machine configuration - does machine have an enclosed cab or not
31	Engine_Horsepower	machine configuration - engine horsepower rating
32	Hydraulics	machine configuration - type of hydraulics
33	Pushblock	machine configuration - option
34	Ripper	machine configuration - implement attached to machine to till soil
35	Scarifier	machine configuration - implement attached to machine to condition soil
36	Tip_control	machine configuration - type of blade control
37	Tire_Size	machine configuration - size of primary tires
38	Coupler	machine configuration - type of implement interface
39	Coupler_System	machine configuration - type of implement interface
40	Grouser_Tracks	machine configuration - describes ground contact interface
41	Hydraulics_Flow	machine configuration - normal or high flow hydraulic system
42	Track_Type	machine configuration - type of treads a crawler machine uses
43	Undercarriage_Pad_Width	machine configuration - width of crawler treads
44	Stick_Length	machine configuration - length of machine digging implement
45	Thumb	machine configuration - attachment used for grabbing
46	Pattern_Changer	machine configuration - can adjust the operator control configuration to suit the user
47	Grouser_Type	machine configuration - type of treads a crawler machine uses
48	Backhoe_Mounting	machine configuration - optional interface used to add a backhoe attachment
49	Blade_Type	machine configuration - describes type of blade
50	Travel_Controls	machine configuration - describes operator control configuration
51	Differential_Type	machine configuration - differential type, typically locking or standard
52	Steering_Controls	machine configuration - describes operator control configuration


## Steps to run:
* Create a conda environment with scikit-learn, numpy, matplotlib, jupyter, pandas, seaborn
* Clone this repo
* Run the notebook

## License
This notebook is created by Abhishek Gautam and is licenced under MIT.

