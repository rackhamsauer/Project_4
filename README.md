# Automated Account (Bot) Identifier

## Team Introduction

This project would not exist if not for the tireless work of the following team members:

**Judith Cuellar**

**Juliet Messier**

**Micheal McCloskey**

**Seren Frazin**

**Stacie Sauer-Rackham**

## Project Overview 
We have developed a machine learning model that identifies the presence of **Automated Account (Bot)** on Twitter. 

Bots undermine the authenticity of interactions on social media platforms. Bots can disseminate misinformation, manipulate trends, and push malicious links&mdash; all of which is harmful to public discourse. 

With the aid of our model, we can battle back the threat of bots on Twitter. 

For more information about Bots, please refer to the following sources:
+  [Twitter Bot&mdash; Wikipedia](https://en.wikipedia.org/wiki/Twitter_bot#:~:text=An%20X%20bot%2C%20formerly%20known,or%20direct%20messaging%20other%20accounts.)
+  [What are Twitter bots, and why is Elon Musk obsessed with them?](https://www.cbsnews.com/news/elon-musk-twitter-bots-cbs-explains/)


### Project Question
Can we accurately identify if a twitter account is a Bot account?

### Index

+ [Data Sources](#data-sources)
    + [Data Exploration](#data-exploration)
+ [Tools](#tools)
    + [Data Transformation Tools](#data-transformation-tools)
    + [Database Tools](#database-tools)
    + [Machine Learning Tools](#machine-learning-tools)
    + [Dashboard Tools](#dashboard-tools)
+ [Machine Learning Model](#machine-learning-model)
    + [Random Forest](#random-forest)
    + [GBM](#gbm)
    + [Tensor Flow](#tensor-flow)
    + [Logistic Regression](#logistic-regression)
    + [KNN](#knn)
    + [Conclusions](#conclusions)
+ [Statistical Analysis](#statistical-analysis)
    + [Follower Activity Analysis](#follower-activity-analysis)
    + [Geo Location Analysis](#geo-location-analysis)
    + [Median Follower Analysis](#median-follower-analysis)
    + [Verified Account Analysis](#verified-account-analysis)
+ [Database](#database)
+ [Tableau Dashboard](#tableau-dashboard)
+ [Presentation](#presentation)

### Project Outline

![Outline of project highlights](https://github.com/rackhamsauer/Project_4/blob/main/Screenshots/Project%204%20Outline.png)

## Data Sources
The following sources will be merged in python to create a robust dataset for analysis:

+ [Twitter Human Bots Dataset](https://www.kaggle.com/code/davidmartngutirrez/bots-accounts-eda/data?select=twitter_human_bots_dataset.csv)&mdash; 37438 rows of data collected from the Twitter API.

+ [Cresci-2017 Dataset](https://botometer.osome.iu.edu/bot-repository/datasets.html)&mdash; an annotated dataset of real and Bot accounts from the Bot Repository. 

### Data Exploration
Our team cleaned these datasets by dropping irrelevant columns, clarifying column names, dropping null values, and converting values to numeric booleans. Once done, we exported the data into a [downloadable csv file](Data/clean_data.csv). 

## Tools
We used the following tools throughout our project:

### Data Transformation Tools

+ Python&mdash; Pandas, Jupyter Notebook 

### Database Tools

+ SQL

+ Microsoft Excel

### Machine Learning Tools

+ Python&mdash; Pandas, PySpark, Jupyter Notebook, Pathlib, Sklearn, Matplotlib, Tensorflow, Keras, Numpy, Google Colab

### Dashboard Tools

+ Tableau

## Machine Learning Model
To create the most accurate model for identifying Bot accounts, our team tested the following five Machine Learning Models:
+ Random Forest
+ GBM
+ Tensor Flow
+ Logistic Regression 
+ KNN 

All of our models exceeded 70% accuracy in identifying bot activity. The following chart shows how well each model performed:
![screenshot of model performance](https://github.com/rackhamsauer/Project_4/blob/main/Screenshots/Machine%20Learning%20Model%20Performance.png)

### Random Forest
Our Random Forest model performed the best out of all our models. It was able to identify bots with 88% accuracy. Our Random Forest model found the following factors to be the most influential in identifying bots:
![screenshot of Random Forest performance](https://github.com/rackhamsauer/Project_4/blob/main/Screenshots/Random%20Forest%20Screenshot.png)

### GBM 
Our GBM model identified bots with 87% accuracy. Below is information regarding GBM Model precision, recall, f1-score, and support:

![screenshot of GBM performance](https://github.com/rackhamsauer/Project_4/blob/main/Screenshots/GBM%20Model%20Performance.png)

### Tensor Flow
Our Tensor Flow model was able to identify bots with 79% accuracy by its final trial. Below is graph detailing the results of each of our 5 Tensor Flow Trials:
![screenshot of Tensor Flow Trials](https://github.com/rackhamsauer/Project_4/blob/main/Screenshots/Tensor%20Flow%20Trials.png) 

### Logistic Regression
Our Logistic Regression model identified bots with 71.5% accuracy. Below is information regarding Logistic Regression precision, recall, f1-score, and support:

![screenshot of logistic Regression performance](https://github.com/rackhamsauer/Project_4/blob/main/Screenshots/Logistic%20Regression%20Screenshot.png)

### KNN 
Our KNN model identified bots with 70.6% accuracy. Below is information regarding KNN precision, recall, f1-score, and support:

![screenshot of KNN performance](https://github.com/rackhamsauer/Project_4/blob/main/Screenshots/KNN%20Performance.png)

### Conclusions
Based on the performance of the various models, our Random Forest model should be used to identify bot activity on Twitter. It was our most accurate model and detailed which factors could be examined to identify bots. Further analysis of these factors should be done to help us better understand the data. 

## Statistical Analysis

After seeing the results of our Random Forest Model, we analyzed follower activity, geolocation, median followers, and verified accounts to better understand how bots differ than human users. Bellow are four charts detailing the results of our analysis:

### Follower Activity Analysis
![Chart of follower activity](https://github.com/rackhamsauer/Project_4/blob/main/Screenshots/Follower%20Activity.png)

### Geo Location Analysis
![Chart of Geo Location](https://github.com/rackhamsauer/Project_4/blob/main/Screenshots/Geo%20Location%20Analysis.png)

### Median Follower Analysis 
![Chart of Median Followers](https://github.com/rackhamsauer/Project_4/blob/main/Screenshots/Median%20Followers%20Dashboard.png)

### Verified Account Analysis
![Chart of Verified Accounts](https://github.com/rackhamsauer/Project_4/blob/main/Screenshots/Verified%20Accounts%20.png)

## Database
We imported our data into a PostgreSQL server. Below is our ERD illustrating how our database is structured:
![Image of ERD](https://github.com/rackhamsauer/Project_4/blob/main/Screenshots/DESCRIPTION_ERD.png)

## Tableau Dashboard
We have used Tableau to create an interactive dashboard that allows users to examine the key factors our model uses to identify Bots on Twitter. Our full Tableau story can be found [here](https://public.tableau.com/app/profile/micheal.mccloskey/viz/shared/FSZS2GDWZ).

## Presentation
A copy of our presentation can be found [here](https://github.com/rackhamsauer/Project_4/blob/main/Bot%20Identification%20Final%20Theme.pptx).
