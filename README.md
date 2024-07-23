# group-eight-project
# FROM SCRIPT TO SCREEN: WHAT MAKES BOX OFFICE HIT?
# 1. Introduction
# 1.1 Overview
Applying exploratory data analysis to provide insights for a Microsoft stakeholder on which types of films to produce.
## 1.2 Business Understanding
*Objective*
The goal of this project is to use exploratory data analysis (EDA) to draw insights to aid the making of a new movie studio looking to enter the film industry and needs to determine which types of films are currently est performing at the box office. By analyzing various datasets related to movie performance. The objective is to identify trends and characteristics of successful films that can guide the studio’s content creation strategy.
*Business context*
With the evolution of film industry, understanding the market and consumer preferences is essential for new entrants. A new movie studio must leverage data-driven insights to make informed decisions about film production. The business wants to identify which factors contribute to box office success to maximize their investment and ensure their film offerings align with market demands.
# 2. Data Understanding
## 2.1 Data
The folder containing the data is called "zippedData" which contains movie datasets from:

1. Box Office Mojo- an online database providing detailed information on box office revenues

2. IMDB- a comprehensive database of movie and TV information

3. Rotten Tomatoes- a review aggregation website for films and TV shows

4. TheMovieDB- a community-driven movie and TV database

5. The Numbers- a database providing box office revenue information and other film metrics

The files are in different formats namely CSV and TSV files and can be opened using the pd.read_csv.
Data from IMDB is in a SQLite Database.

Data from the TSV files was not used because it didn't have the data neede for this analysis. Only the compressed CSV files and unzipped IMDB file were used.

Dataset used has 1001 rows and 10 columns. The columns are:

1. movie - name of film

2. runtime_minutes - total minutes of a film

3. genres - types of films

4. averagerating - average rating of individual films

5. production_budget - total production budget for the film

6. month - release month 

7. profit - total amount remaining production budget from total gross

8. original_language - film language

9. popularity - how popular a film is

10. year - release year 

In order to provide recommendations, this analysis will address the following questions:

1.What genres of films are performing best at the box office?

2.Which languages are most successful in terms of box office revenue?

3.How does the month of release impact profitability?

4.Is there a correlation between the duration of films and other factors?
## 2.2 Loading Libraries
Load the libraries required for the analysis
## 2.3 Loading the Data
Load the compressed CSV files and the IMDB zippedfile. Unpack the IMDB file then query it using SQLite then convert the movie basics tables and movie ratings tables into dataframes.
# Data Cleaning
Here, we will perform data cleaning. This involves preparing the data for analysis by removing irrelevant or incorrect information, which can negatively impact the model or algorithm by reinforcing incorrect assumptions.

We will analyze each of the five datasets separately. Our data cleaning steps include:

1.Completeness - Ensure that the datasets have no missing values.

2.Uniformity - Verify that the data types in the datasets are correct.

3.Consistency - Ensure that there are no duplicate entries in the data.

This process is crucial as clean and accurate data is essential for building reliable and effective models.
