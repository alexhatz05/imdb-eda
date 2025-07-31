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
<img width="989" height="490" alt="Avg Rating per Genre" src="https://github.com/user-attachments/assets/cf112cad-6034-4238-ab2f-942fbb28867e" />

<img width="837" height="550" alt="Correlation of IMDb Score MetaScore with outliers" src="https://github.com/user-attachments/assets/801a04bf-acea-46b0-b37d-8604c91cba81" />

<img width="520" height="433" alt="IMDb MetaScore correlation heatmap" src="https://github.com/user-attachments/assets/5aab8132-daf7-4b15-93e4-3e6e33f771c0" />

<img width="553" height="453" alt="IMDb MetaScore correlation scatter" src="https://github.com/user-attachments/assets/91ea6992-a6e5-48e6-a9a4-8230f5dd8b2f" />

<img width="558" height="457" alt="Rating vs Duration" src="https://github.com/user-attachments/assets/10b3a3c6-b3e3-453e-976b-30ae6541c1e6" />

<img width="558" height="457" alt="Rating vs Duration box plot" src="https://github.com/user-attachments/assets/daa65ea3-c966-4a5c-8113-428463be189c" />

<img width="560" height="432" alt="violin plots" src="https://github.com/user-attachments/assets/df950531-9244-4501-9a54-9e8cee43bf76" />


## 🚀 Getting Started

### Prerequisites

Install the dependencies using pip:

```bash
pip install pandas matplotlib seaborn jupyter

