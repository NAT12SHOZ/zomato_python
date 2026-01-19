# 🍽️ Zomato Data Analysis Project


## Project Overview

This project analyzes the Zomato restaurant dataset across multiple countries to understand restaurant trends such as ratings, votes, online delivery availability, and pricing behavior. The analysis includes data cleaning, merging datasets, feature engineering, and visualization using Python.
The goal is to extract meaningful insights about customer engagement and restaurant performance worldwide. 

![Dashboard](barplot.png)


<img width="1221" height="821" alt="Screenshot 2026-01-19 110405" src="https://github.com/user-attachments/assets/d712c330-dd10-4e03-9959-4f0708a34fb4" />
<img width="1282" height="779" alt="Screenshot 2026-01-19 111008" src="https://github.com/user-attachments/assets/61ec435c-edce-4a0f-9191-99cb0d28b4ab" />

## Project Structure

zomato-project/
            │
     ├── Country-Code.xlsx
     ├── README.md
     ├── ZOMATO PROJECT (1).ipynb
             └── zomato.csv

## Data Set

-	zomato.csv – Contains restaurant information such as ratings, votes, cost, cuisines, and delivery options.
-	Country-Code.xlsx – Maps country codes to country names.
These datasets are merged using the Country Code column to add country names to the Zomato dataset.

## Data Processing And Cleaning

### The following steps are performed:
-	Load both datasets
-	Merge Zomato and Country datasets
-	Standardize column names
-	Create a new feature: price_category
-	Analyze ratings, votes, and delivery behavior
-	Save the final merged dataset
### Example price category logic:
-	Budget → Cost ≤ 500
-	Mid-range → Cost ≤ 1500
-	Premium → Cost > 1500
### The final cleaned dataset is saved as:
  [Download Here](data/processed/zomato_merged_cleaned.csv) 

## Analysis And Visualization

### The notebook explores:
-	Top countries by number of restaurants
-	Countries offering online delivery
-	Average restaurant rating by countries
-	Online delivery vs average rating
-	Price category vs votes and ratings
### Sample insights:
-	India , U.S.A , U.K. contribute more in restaurant business. 
-	In online deliveries India and Dubai take the lead.
-	Restaurants offering online delivery generally perform better in ratings. 
-	Premium restaurants receive higher average votes and ratings. 
-	Country-level trends show differences in service adoption.

## Technology Used

- Excel
- Python
- Pandas
- Matplotlib
- Seaborn
- Google Coolab

## Usage

-	To load the cleaned dataset: 
-	import pandas as pd 
-	df = pd.read_csv("data/processed/zomato_merged_cleaned.csv")

## Author

- Natisha Sameer 
- 9899626704 
- natisha.eajaz1979@gmail.com






