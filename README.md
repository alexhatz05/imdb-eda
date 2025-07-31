# imdb-eda
# 🎬 IMDb Movies – Exploratory Data Analysis (EDA)

This project explores the IMDb movie dataset through visual analysis and statistical exploration using Python. It aims to uncover patterns in ratings, durations, genres, metascores, and other movie characteristics.

## 📌 Objective

To perform a structured exploratory data analysis (EDA) on a movie dataset containing IMDb ratings, Metascore, Duration, Genre, and other attributes. The goal is to discover insights and relationships between variables such as:

- Do longer movies get better ratings?
- Is there a correlation between IMDb Rating and Metascore?
- How does survival (or success) relate to movie duration, genre, or other features?

## 🗂 Dataset

The dataset includes the following columns (or similar):

- `Title` – Movie title
- `Genre` – Genre(s) of the movie
- `Duration` – Duration in minutes
- `IMDb Rating` – Audience rating from IMDb
- `Metascore` – Critic score (0–100)
- `Votes` – Number of votes on IMDb
- `Year` – Release year
- and possibly others depending on version.

Format: CSV  
Source: Course-provided or IMDb-style data

## 🔍 Steps Performed

1. **Data Cleaning**
    - Removed duplicates
    - Filled missing values
    - Converted durations to numeric
    - Created categorical duration groups

2. **Feature Engineering**
    - Grouped durations into `Short`, `Medium`, `Long`, `Epic`
    - Created `RatingDiff` (IMDb - Metascore)

3. **Visualization & Analysis**
    - Correlation matrix
    - Scatter plots (e.g., IMDb vs Metascore, IMDb vs Duration)
    - Boxplots and violin plots by duration group
    - Survival/ratings breakdown by gender, class, genre
    - Distribution histograms for age/duration/etc.

## 📊 Key Insights

- **Positive correlation** between IMDb Rating and MetaScore (~0.75)
- **Longer movies** tend to receive **higher ratings**
- **Epic-length movies** (over 150 mins) consistently have **strong ratings**
- Clear genre-based variation in rating distribution

## 🛠 Technologies

- Python 3.x
- Jupyter Notebook
- Pandas
- Matplotlib
- Seaborn

## 📷 Example visualizations
![img.png](img.png)

![Correlation of IMDb Score MetaScore with outliers.png](images/Correlation%20of%20IMDb%20Score%20MetaScore%20with%20outliers.png)

![IMDb MetaScore correlation heatmap.png](images/IMDb%20MetaScore%20correlation%20heatmap.png)

![IMDb MetaScore correlation scatter.png](images/IMDb%20MetaScore%20correlation%20scatter.png)

![Rating vs Duration.png](images/Rating%20vs%20Duration.png)

![Rating vs Duration box plot.png](images/Rating%20vs%20Duration%20box%20plot.png)

![violin plots.png](images/violin%20plots.png)


## 🚀 Getting Started

### Prerequisites

Install the dependencies using pip:

```bash
pip install pandas matplotlib seaborn jupyter

