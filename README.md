# Sales Data Analysis - Answering real world business questions

## Introduction :
### In this project we use Pandas & Seaborn to analyze and answer business questions about 12 months worth of sales data. The data contains thousands of electronics store purchases broken down by month, product type, cost, purchase address, etc.

## Code and Resources Used :

#### Python Version : 3.8.5
#### Libraries Used : pandas, numpy, seaborn, plotly, os, itertools, collections
#### Data : [Kaggle - Monthly Sales 2019](https://www.kaggle.com/zaimeali1997/monthly-sales-2019)

## The project consists of two parts :
* Data Cleaning
* Data Analysis

## Data Cleaning :
* Drop NaN values from DataFrame
* Removing rows based on a condition
* Change the type of columns (to_numeric, to_datetime, astype)
* Extracting additional features from existing columns :
  * Month, Day of week, Hour from Order Date
  * State, City, Zip Code from Purchase Address
* Creating Total sales amount column

## Data Analysis :
### Here we explore 5 high level business questions related to our data.

### 1. What were the best months for sales? How much was earned in those month?
![best months for sales](https://raw.githubusercontent.com/ritik-k/electronics_store_analysis/master/plots/month.png)

### We can see that January is the worst month for Sales and December is the best month. We also see that sales keep increasing till April after which they start decreasing again; this is interesting and further analysis can be done on this, we can try to a correlation to the marketing and advertisement budget. It is seen that the months of October, November and December report good sales and it is expected as these months contain most of the major US holidays such as Halloween, Thanksgiving Day, Cyber Monday, Black Friday Sale and Christmas. People usually buy a lot of gifts during these holidays.

### 2. Which city had the best sales?
![best city for sales](https://raw.githubusercontent.com/ritik-k/electronics_store_analysis/master/plots/city.png)

### San Francisco is the best city for sales which make sense because Silicone Valley is located here which employs some of the world's best IT employees who tend to use more electronic items. We can also look at further questions such as the amount of marketing and advertisement budget to determine why cities such as Portland and Austin are performing poor as compared to other cities.

### 3. What time should we display advertisements to maximize the likelihood of customers buying the product? ( Best Time for Sales )
![best time for sales](https://raw.githubusercontent.com/ritik-k/electronics_store_analysis/master/plots/hour.png)

### Here we can see that 12PM and 7PM are the two hours during which we have the highest sales. This makes sense because these are the hours during which people are generally going to or returning from work. Thus if we ran an advertisement during these 2 hours, it will get maximum visibility and in turn increase the chance of customers buying the product.

### 4. What products are most often sold together?
![most often sold together](https://raw.githubusercontent.com/ritik-k/electronics_store_analysis/master/plots/2_product.png)

### This data is very useful as using this we can create offers or promotions which can increase our sales further. When a person buys a phone we can offer a Lightning Charging Cable or a Wired Headphones at a discounted price which will push more customers to buy these products.

### 5. Which products sold the most? Why?
![best products](https://raw.githubusercontent.com/ritik-k/electronics_store_analysis/master/plots/product.png)

### Here we can see that products that are generally cheap, viz AA, AAA Batteries, Charging Cable or Headphones are sold more frequently as compared to other expensive products. People buy these products more as batteries need to be replaced and charging cables and headphones are generally of a lower quality and need replacemnet.

___
### Usage :
#### This project is best viewed in a notebook viewer, which can be accessed [here](https://nbviewer.jupyter.org/github/ritik-k/electronics_store_analysis/blob/master/sales.ipynb). In this notebook, you will find a walk through of the work done, detailed analysis and the respective code.