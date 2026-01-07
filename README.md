# 🎬 Netflix Data Analysis Project

Welcome to the **Netflix Data Analysis Project**! This repository is dedicated to exploring and analyzing the vast library of content available on Netflix. By leveraging data analysis techniques, we aim to uncover trends, user preferences, and insights into the world of streaming entertainment.

## 📂 Project Structure

The core analysis is contained within the `Netflix data/` directory:

-   **`data.ipynb`**: The Jupyter Notebook acts as the heart of this project. It contains the complete end-to-end analysis pipeline, including:
    -   Data Loading and Inspection
    -   Data Cleaning and Preprocessing
    -   Feature Engineering
    -   Exploratory Data Analysis (EDA) and Visualizations
-   **`mymoviedb.csv`**: The primary dataset used for this analysis, containing rich metadata about movies and TV shows such as titles, release dates, popularity scores, vote counts, averages, and genres.

## 🛠️ Analysis Workflow

The `data.ipynb` notebook follows a structured approach to derive insights:

1.  **Data Loading & Overview**:
    -   The dataset is loaded using **Pandas**.
    -   Initial inspection using `df.head()`, `df.info()`, and `df.describe()` to understand data types, missing values, and statistical distributions.

2.  **Data Cleaning**:
    -   **Date Formatting**: Converting `Release_Date` to datetime objects and extracting the release year for trend analysis.
    -   **Handling Duplicates**: Checking for and removing duplicate entries to ensure data integrity.
    -   **Missing Values**: Identifying and handling null values (e.g., dropping rows with missing critical data).

3.  **Feature Engineering**:
    -   **Vote Categorization**: Creating a new category for `Vote_Average` to classify content into buckets like 'Not_popular', 'Below_avg', 'average', and 'popular'.
    -   **Genre Explosion**: Since movies can belong to multiple genres (comma-separated), the `Genre` column is "exploded" to allow for accurate counts and analysis of individual genres.

4.  **Visualizations & Insights**:
    -   **Genre Distribution**: Using **Seaborn** (`sns.catplot`) to visualize the frequency of different genres.
        -   *Key Insight*: The analysis identifies the most frequent genres, with **Thriller** appearing as a top contender in the dataset glimpse.
    -   **Popularity Trends**: (Planned/In-progress) Analysis of how popularity varies across different genres and release years.

## 🚀 Future Scope

> **Note:** Currently, this project features **only Netflix data analysis**.

We have an exciting roadmap ahead! In future updates, we plan to expand this repository to include comprehensive analyses of data from **more platforms**, such as:

-   **Amazon Prime Video**
-   **Hulu**
-   **Disney+**
-   **HBO Max**

Stay tuned for cross-platform comparisons and deeper dives into the streaming landscape!

## 💻 Tech Stack

-   **Python**
-   **Pandas** (Data Manipulation)
-   **NumPy** (Numerical Computing)
-   **Matplotlib & Seaborn** (Data Visualization)
-   **Jupyter Notebook** (Interactive Environment)

## 🏃‍♂️ How to Run

1.  Clone this repository.
2.  Navigate to the `Netflix data` directory.
3.  Launch Jupyter Notebook: `jupyter notebook data.ipynb`.
4.  Run the cells sequentially to reproduce the analysis.
