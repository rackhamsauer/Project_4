# Automated Account (Bot) Detection 

## Team Introduction

This project would not exist if not for the tireless work of the following team members:

**Judith Cuellar**

**Juliet Messier**

**Micheal McCloskey**

**Seren Frazin**

**Stacie Sauer-Rackham**

## Project Overview 
We have developed a machine learning model that predicts the frequency of **Automated Account (Bot)** creation on Twitter. 

Bots undermine the authenticity of interactions on social media platforms. Bots can disseminate misinformation, manipulate trends, and push malicious links&mdash; all of which is harmful to public discourse. 

With the aid of our model, we can battle back the threat of bots on Twitter. 

### Project Question
Can we predict the rates at with new Bot accounts are created on Twitter by using a machine learning model?

### Index

+ [Data Sources](#data-sources)
    + [Data Exploration](#data-exploration)
+[Tools](#tools)

### Project Outline

~~We will add a visualized outline later~~

## Data Sources
The following sources will be merged in python to create a robust dataset for analysis:

+ [Twitter Human Bots Dataset](https://www.kaggle.com/code/davidmartngutirrez/bots-accounts-eda/data?select=twitter_human_bots_dataset.csv)&mdash; 37438 rows of data collected from the Twitter API.

+ [Cresci-2017 Dataset](https://botometer.osome.iu.edu/bot-repository/datasets.html)&mdash; an annotated dataset of real and Bot accounts from the Bot Repository. 

### Data Exploration
Our team cleaned these datasets by dropping irrelevant columns, clarifying column names, dropping null values, and converting values to numeric booleans. Once done, we eported the data into a [downloadable csv file](Data/clean_data.csv). 

## Tools
We used the following tools throughout our project:

**Data Transformation**

+ Python&mdash; Pandas, Jupyter Notebook 

**Database**

+ SQL

+ Microsoft Excel

**Machine Learning Model**

+ Python&mdash; Pandas, PySpark, Jupyter Notebook

**Dashboard**

+ Tableau

