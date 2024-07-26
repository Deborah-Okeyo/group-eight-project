# group-eight-project
# FROM SCRIPT TO SCREEN: WHAT MAKES BOX OFFICE HIT?
# Project By

1.David Chege

2.Evans Oyugi

3.Deborah Okeyo

Marion Macharia

# 1. Introduction
![pexels-hatice-796619215-27219316](https://github.com/user-attachments/assets/eb85b286-1b8e-472d-860d-86cbd9694dcf)
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

# Results
## Genres

![Most Profitable Genres](https://github.com/user-attachments/assets/01438494-b275-49e0-ba73-f533c64e38c0)

The top 5 most profitable genres are Adventure, Action, Comedy, Drama and Animation.

## Languages

![Most_Profitable_Languages](https://github.com/user-attachments/assets/7cd72d5d-2807-498b-80f8-e4b5d2709e35)

The top 5 most profitable languages are Thai, Telugu, English, Hungarian and Hindi

## Month of Release

![Most_Profitable_Months](https://github.com/user-attachments/assets/5a23394d-4715-42db-9670-ffd83984be14)

The top 3 most profitable months are June, May, July, November and December.

# Correlation

![Correlation Representation Using a Heatmap](https://github.com/user-attachments/assets/a1712482-e6c6-4d65-b571-515c79039ea2)

We observe a positive correlation among all the variables, though the strength of these correlations varies. A positive correlation indicates that as one variable increases, the other variable also tends to increase, demonstrating a direct relationship between the two. For example, if one variable shows an upward trend, the correlated variable typically follows suit.

# Conclusion
## 1. What genre of films are performing best at box office?
The genres were analyzed based on profit, budget, popularity, and rating. To determine the best-performing genres, we combined the top three from each of these categories. These genres are Adventure, Action, Comedy, and Drama. However, the heatmap shows that rating has a weak correlation with profit and popularity, so we will not consider rating in our final assessment. Since higher budgets correlate with higher popularity and profit, the top genres are Adventure, Action, and Comedy.

## 2. Which languages are most successful in terms of box office revenue?
The languages were analyzed based on profit, popularity, budget, and rating. To identify the top-performing languages, we combined the top three from each of these categories. The top languages are Thai, Telugu, English, Danish, Modern Greek, German, and Spanish. Considering both profit and popularity, the best languages for films are Thai, Telugu, and English.

## 3. How does the month of release impact profitability?
The release months with the highest profits are June, May, July, November, and December. These months coincide with school breaks and work vacations, which likely contributes to the higher profitability of movies released during these periods. Families and individuals tend to have more free time during these months, leading to increased movie attendance and higher box office revenues.

## 4. Is there a correlation between the duration of films and other factors?
No, runtime minutes for a film have a weak positive correlation with the quantitative variables, so we cannot use it for our analysis. The runtime does not significantly impact a film's profitability or popularity, meaning the duration can vary. Therefore, it will not be included in our recommendations.

# 6. Recommendations
1.The ideal genres to produce are Adventure, Action, and Comedy.

2. The optimal languages for these films are Thai, Telugu, and English. 

3.The best months to release these films are June, May, and July.

# Project Dashboard

For more detailed insights, visit our [Tableau Dashboard](https://public.tableau.com/views/Phase2Dashboard_17218944880860/Dashboard1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link).

# Project Presentation

To view the detailed presentation of our findings, please visit the [Project Presentation](https://public.tableau.com/views/Phase2Dashboard_17218944880860/Dashboard1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link).




