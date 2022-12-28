# Section 2: Introduction to Life-Cycle of Machine Learning Project

### Use case

ex. Predict a person is diabetic or not

In order to perform this, we need data



### Business Understanding

How are you going to gather all the requirements to collect data



### Data Finding

BA and DE send all the requirements to data analysists and give some amazing insight. 

Big Data Engineer is going to take all the raw data and transform the data.

But the data is not going to be in the right format to put into as an input for the machine learning algorithm. Hence, the data need to be cleaned and this process is called the Data Cleaning.

* Are there any missing values?

After the cleaning, we have to do something known as Feature engineering.

Feature engineer is going to transform the data so that it could be in the right format.

What will happen in feature engineering?

* Gender
  * male
  * female

These data are strings. But machine learning deals with numbers. Hence, we have to convert the data. 



# Project #1: Predict the Cancellation of Hotel Booking

## How to read data

Goal: Predict whether a customer is going to cancel the booking or not

Life Cycle

1. Data collection

Various forms such as

* csv/tsv
* json
* dbs
* sql => tale centric / no-sql => document centric 
* web scraping

2. Data Cleaning / Pre-processing / wranging
3. EDA => analyzing data
4. Feature Engineering
5. Machine Learning algorithm to build a model
6. Optimize the model / Hypertune the model



Pandas is all about 1-D or 2-D data structure

1-D : series (array, sequence of numbers)

2-D : Dataframe (table)

## Data Cleaning

You have to clean data so that you can perform data analysis.

Various categories.

- Missing value in our data
- Data type is right or wrong
- any structural error?
- duplicate values or observations in our data

### Missing value

Two ways to deal with

* Delete
  * you might lose important information

After droping the data, let's fill in with the **mode**



Next, drop irrelevant data.

For example, adults, children, and babies. All these values cannot be 0 at the same time.

mode: which subcategory has highest count.

* Fill in
  * various techniques



## Analyzing Demand of Hotels

 Data analysis: Trying to understand the data

Let's say we extract two important features from the data: country and total # of people from that country.

To visualize this, we can map it.

### Geographical Analysis

Plot all the things on a map. How to plot a geographical map?

We have a module called plotly.

Before utilizing, have to install it. Then, establish the setup. 



## Analyzing Prices of Hotels across Year

1. How much do guests pay for a room per night?

Since most of the guests come from the European country, let's assume the currency to be European currency.

Two features: room, avg-price

Mean vs Median

- Mean can badly affect the avg-price. For example, some really big number.

### Quantile

Percentile: assume we have an array of [0,1,2,3,4,5,6,7,8,9]. If we say 1 is the 10th percentile, what it means is that 10% is below 1 and 90% is above 1.

50% is median.



We typically need (Med, Q1, Q3) -> we can plot these values by using box plot.



## Analyzing Demand of Hotels

2. Which are the most busy month?

What features do we need? Month, Rush-City, Rush-R esort

Let's use line chart for this one because it shows the trend well.





## Analyzing which month has highest avg. daily rate?

Two features : Month, adr.

This can be one of the sources to predict the hotel booking.



## Analyzing whether bookings were made only for weekdays or for weekends or for both ??

What type of data do we need?

Matrices: Row (months) columns (features)

We can implement this data using stacked chart 



## How to create useful features for machine learning model

How to create more features to improve our model. For example, using three features: adults, childrent, babies to create a new feature: family.

After creating such useful features, we can drop the original ones that are not needed anymore in the future.



## How to apply feature encoding on Categorical data

We have to convert some data into integer or any other numerical format in order to make it possible for our ML algorithm to work. => This process is called feature encoding.

Categorical => feature encoding => numerical data

We are going to perform mean encoding.
