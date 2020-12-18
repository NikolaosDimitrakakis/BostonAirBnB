# BostonAirBnB
Analysis on Boston AirBnB dataset

### Table of Contents

1. [Installation](#installation)
2. [Project Motivation](#motivation)
3. [File Descriptions](#files)
4. [Results](#results)
5. [Licensing, Authors, and Acknowledgements](#licensing)
6. [CRISP-DM process](#CRISP-DM)

## Installation <a name="installation"></a>

There should be no necessary libraries to run the code here beyond the Anaconda distribution of Python.  The code should run with no issues using Python versions 3.*.

## Project Motivation<a name="motivation"></a>

For this project, I was interestested in using Boston AirBnB data from 2017 to understand:

1. Who host has the more listings in Boston and their price?
2. To take a brief look at response time, response rate and acceptance rate of the hosts.
3. How location affecting price? 
4. The price is related to room type?
5. How the bed type is connected to price? 
6. Can we predict the price?



## File Descriptions <a name="files"></a>

There are 3 notebooks available here with work related to the above questions.  Each of the notebooks is exploratory in searching through the data pertaining to the questions showcased by the notebook title.  Markdown cells were used to assist in walking through the thought process for individual steps.  

## Results<a name="results"></a>

The main findings of the code can be found at the post available [here](https://nikdimi.medium.com/what-can-we-found-from-the-boston-airbnb-dataset-f2507e75b57c).

## Licensing, Authors, Acknowledgements<a name="licensing"></a>

Must give credit to Airbnb Inside for the data.  You can find the Licensing for the data and other descriptive information at the Kaggle link available [here]( https://www.kaggle.com/airbnb/boston).  Otherwise, feel free to use the code here as you would like! 

## CRISP-DM process <a name="CRISP-DM"></a>

1. Business Understanding

Who host has the most listings and what is the average price of the host?
Which of the host has higher metrics in terms of response time, acceptanse rate, and response rate?
Which neighbourhoods are the most expensive and which the cheapest ones?
Which types of property, room and bed are having higher price?
How well can we predict a listing's salary? 
2. Data Understanding

Here we used the Boston AirBnb data to attempt to answer our questions of interest. In this case, using the data to help us arrive at our questions of interest. The complete dataset has three CSV files, we used listing CSV to answer our question since it contains much more information regarding listings, hosts, price, location.

3. Prepare Data

Here we is the stage where we need to prepare our data to answer our questions. We have found in columns missing values, and fillen with the median, we have change data type in the needed columns, and removed symbols from data points. Also we worked with categorical variables and transform them to dummy variables with encoding.

4. Model Data

We were finally able to model the data, but we had some back and forth with step 3. before we were able to build a model that had okay performance. There still may be changes that could be done to improve the model we have in place. From additional feature engineering to choosing a more advanced modeling technique, we did little to test that other approaches were better within this lesson.

5. Results

We found some of the hosts in Boston, their average price, how many listing they have, and used some metrics to see how the hosts performing. There are five hosts with more than fifty listings, Kara has the most with 136 and Alicia has only 50 listings. The highest average price is for Mike and the lowest for Alicia. Most of the hosts around 85% they are responding within a few hours, with 45% of them within an hour. 15% of the host are responding within the day and only 1.5% they need a few days or more to respond. There are three hosts with more than 95% rate: Mike, Kara, Alicia. Flatbook and Alicia are having more than 30 listings and acceptance rates above 90.  Good job Alicia! Then looked at the price and some features connected to price. South Boston Waterfront is the most neighbourhood and the cheapest is Hyde Park. Apartments are dominating the property type. The room type Entire home/apt has the highest mean price, and of course, the real bed is what someone would prefer to stay in!
In the final we tried to predict the price, it is something to predict it but on what we had our model explained 52.2% of the variability in price.
