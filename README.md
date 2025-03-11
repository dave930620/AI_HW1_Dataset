# IMDb Movie Ratings Dataset

## Description
This dataset contains IMDb movie ratings along with their associated genres. Each movie is labeled with multiple genres in a one-hot encoded format. The dataset is designed for machine learning tasks, including supervised regression (predicting ratings) and classification (predicting genres).

## Data Type
- **Format:** CSV (Comma-Separated Values)
- **Columns:**
  - `Movie Name` (string): The name of the movie.
  - `Rating` (float): IMDb rating of the movie (0 to 10).
  - `Action`, `Comedy`, `Drama`, `Horror`, `Science Fiction`, `Mystery`, `Romance`, `Music`, `Animation`, `Adventure`, `Documentary`, `Family`, `Crime`, `Fantasy`, `History`, `Western` (binary 0/1): Genre labels, where 1 indicates the presence of that genre.

## External Source
- Data collected from IMDb (https://www.imdb.com/) using web scraping techniques.

## Amount and Composition
- **Total Movies:** 1000
- **Columns:** 18 (1 name, 1 rating, 16 genre labels)
- Each row represents one movie, with multiple genres assigned in a **one-hot encoded format**.

## Conditions for Data Collection
- Only movies with an IMDb rating are included.
- Movies must have at least one genre assigned.
- Movies released between 2000 and 2024 are included.

## Data Collection Process
- **Web Scraping:** Used `BeautifulSoup` and `requests` in Python to extract movie names, ratings, and genres from IMDb.
- **Data Cleaning:** remove empty entries and format categorical labels into a one-hot encoding format.

## Example
```csv
Movie Name,Rating,Action,Comedy,Drama,Horror,Science Fiction,Mystery,Romance,Music,Animation,Adventure,Documentary,Family,Crime,Fantasy,History,Western
Citizen Nawi,7.6,0,0,0,0,0,0,0,0,0,0,1,0,0,0,0,0
Inception,8.8,1,0,1,0,1,0,0,0,0,1,0,0,0,0,0,0
The Dark Knight,9.0,1,0,1,0,0,0,0,0,0,0,0,0,1,0,0,0
