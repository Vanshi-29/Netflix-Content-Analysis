# Netflix Movies and TV Shows Content Analysis

## Project Overview

This project analyzes Netflix Movies and TV Shows using Exploratory Data Analysis (EDA), data visualization, feature engineering, and machine learning.

The main objective is to understand Netflix's content catalog, identify useful patterns and trends, and build a classification model to predict whether a title is a Movie or TV Show.

## Dataset

The dataset contains 8,807 Netflix titles and 12 columns, including:

- Type
- Title
- Director
- Cast
- Country
- Date Added
- Release Year
- Rating
- Duration
- Genres
- Description

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Analysis Performed

The project includes:

- Dataset exploration and statistical analysis
- Missing-value analysis and data cleaning
- Duplicate and outlier analysis
- Movies vs TV Shows analysis
- Content addition trends
- Country-wise content analysis
- Genre analysis
- Rating distribution
- Movie duration analysis
- TV Show season analysis
- Director analysis
- Correlation analysis

## Feature Engineering

Three meaningful features were created:

- `content_age` – age of the content based on its release year
- `genre_count` – number of genres/categories associated with a title
- `is_indian` – indicates whether India is associated with the title's country information

## Machine Learning

The project uses an 80:20 train-test split and compares two classification models:

- Logistic Regression
- Decision Tree

One-Hot Encoding was used for categorical rating features, and feature scaling was applied where required.

### Model Results

| Model | Accuracy | F1 Score |
|---|---:|---:|
| Logistic Regression | 71.62% | 0.408 |
| Decision Tree | 71.62% | 0.372 |

Logistic Regression performed better based on F1 Score.

## Key Insights

- Movies represent approximately 69.6% of the titles, while TV Shows represent approximately 30.4%.
- Netflix content additions reached their highest level in 2019.
- International Movies and Dramas are among the most common content categories.
- TV-MA and TV-14 are the most common ratings.
- TV Shows are strongly concentrated around shorter series, with one-season shows being the most common.

## Recommendations

1. Continue investing in international and region-specific content.
2. Maintain a strong movie catalog while continuing to expand TV Show content.
3. Consider audience-focused content planning based on rating and content preferences.

## Project Files

- `Netflix_Content_Analysis.ipynb` – complete Jupyter Notebook containing the analysis and machine learning workflow.
- `netflix_titles.csv` – dataset used for the analysis.
