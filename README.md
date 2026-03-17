# Movie Industry Correlation Analysis

This project explores a comprehensive dataset from the movie industry to identify the key variables (such as budget, user votes, genre, etc.) that have the strongest correlation with a film's financial success, measured by its gross earnings at the box office.

### Project Structure

* `Movie correlation project.ipynb`: The main analysis notebook, featuring:
    * **Data Cleaning & Pre-processing**: Inspection of missing values, data type validation, and conversion of categorical variables into numerical codes (`cat.codes`) to enable mathematical correlation calculations.
    * **Exploratory Data Analysis (EDA)**: Use of scatter plots and regression plots to visually assess the relationship between budget and gross earnings using Matplotlib and Seaborn.
    * **Correlation Analysis**: Implementation of correlation matrices using Pearson, Kendall, and Spearman methods.
    * **Visual Insights**: Development of a Correlation Heatmap to identify top-performing feature pairs.
* `requirements.txt`: List of Python libraries required to run the analysis (Pandas, NumPy, Seaborn, Matplotlib).

### Dataset Overview

**Input Variables (Movie Features):**
* `name`: Title of the movie.
* `rating`: Content rating (e.g., R, PG-13).
* `genre`: Movie category.
* `year`: Release year.
* `released`: Release date and country.
* `score`: Average user rating (e.g., IMDb score).
* `votes`: Total number of user votes.
* `director/writer/star`: Key creative personnel.
* `country`: Country of production.
* `budget`: Production cost.
* `company`: Production studio.
* `runtime`: Duration in minutes.

**Target Variable:**
* `gross`: Total box office earnings.

### Key Results
The correlation analysis yielded the following insights:
* **Budget and Votes**: These variables show the highest and most significant correlation with gross earnings.
* **Critical Score**: Contrary to common assumptions, a movie's score has a relatively low impact on its actual financial performance.
