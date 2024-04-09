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
+ [Database](#database)
+ [Tableau Dashboard](#tableau-dashboard)
+ [Presentation](#presentation)

### Project Outline

~~We will add a visualized outline later~~

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

### Random Forest
Our Random Forest model performed the best out of all our models. It was able to identify bots with 88% accuracy. Our Random Forest model found the following factors to be the most influential in identifying bots:
![screenshot of Random Forest performance]()

### GBM 

### Tensor Flow

### Logistic Regression

### KNN 

## Database
We imported our data into a PostgreSQL server. Below is our schema illustrating how our database is structured:
## Tableau Dashboard
We have used Tableau to create an interactive dashboard that allows users to visualize the key factors our model uses to identify Bots on Twitter. Our full Tableau story can be found [here](https://public.tableau.com/app/profile/micheal.mccloskey/viz/TwitterBotAnalysis/Story1).

## Presentation
