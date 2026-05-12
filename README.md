## Title: 
Film Genre Tracking

## Description: 
This project is meant for tracking the popularity of film genres across the past decade. Popular genres are tracked through various data points including: highest grossing in the U.S. box office, highest audience ratings, and award ceremony nominations. The project looks at the time period from 2015/16-2025/26 to see how certain genres perform over the years, ultimately tracking the percent of change for each genre.


## Rationale:
Movies are often reflective of society, so when certain genres become popular, it can be indicative of cultural attitudes during a specific time period. For example, during World War 1 propaganda films, including spy movies, became really popular to boost American citizens’ morale and support for the military. This project aims to see if current genre trends can give insight to how Americans are feeling culturally today.

## Workflow:
* Extract top 10 highest rated films with genre IDs from 2015-2026 using the TMDb API and export it as a CSV, use search and replace in Excel to convert genre ID numbers into words.
* Extract top 10 highest grossing films from 2015-2026 using the unofficial BoxOffice Mojo API and export it as a CSV file.
* Create a file of Academy Award nominees and winners from 2016-2026 from major categories (including but not limited to Best Picture, Best Actor/Actress, Best Screenplay - Original/Adapted) and convert to CSV.
* Download Golden Globes dataset from Kaggle and extract nominees and winners in major categories (including but not limited to Best Picture - Drama/Comedy, Best Actor/Actress, Best Screenplay) from the years 2016-2020, supplement 2021-2026 data from the Golden Globes website in Excel and convert to CSV.
* Source genres for all films from AA, GG, and BoxOffice Mojo from the IMDb website.
* Clean the data into a usable dataset using a combination of Open Refine and Excel.
* Analyze and visualize all datasets using Pandas and MatPlotLib libraries to search for genre trends.

Tools Used:
* TMDb API
* Unofficial BoxOffice Mojo API
* Academy Awards database
* Kaggle dataset (for Golden Globes data)
* 'pandas' python library
* 'matplotlib' python library
* OpenRefine
* Excel

## Further Uses:
This project can be reused and expanded on in the future to continue tracking genre trends. All API coding should be reusable to make calls for extracting the highest-rated and highest-grossing films from TMDb and BoxOffice Mojo. The Golden Globes and Academy Awards databases update each year after their respective ceremonies and the spreadsheets should be updated accordingly. Additionally, all Python code should be reusable for creating visualizations for the data extracted. This will allow anyone to be abe to continue tracking genre popularity for future films.

## Files List:
* tmdb_data.ipynb - Python notebook with TMDb API call to get top 10 highest rated films from 2015-2025
* tmdb_visualizations.ipynb - Python notebook with visualizations created from TMDb data
* 2026-04-28_tmdb_v2.csv - Cleaned TMDb data with genres
* tmdb_visualizations folder - All visualizations created as jpg files
* boxoffice_data.ipynb - Python notebook with unofficial BoxOffice Mojo API call to get top 10 highest grossing films from 2015-2025
* boxoffice_visualizations.ipynb - Python notebook with visualizations created from BoxOffice Mojo data
* 2026-04-30_boxoffice_v2.csv - Cleaned BoxOffice Mojo data with genres
* boxoffice_visualizations folder - All visualizations created as jpg files
* 2026-05-04_academy_awards_genre.csv - Cleaned Academy Awards data with genres
* oscars_visualizations.ipynb - Python notebook with visualizations created from Academy Awards data
* oscars_visualizations folder - All visualizations created as jpg files
* 2026-05-02_golden_globes_genre.csv - Cleaned Golden Globes data with genres
* globes_visualizations.ipynb - Python notebook with visualizations created from Golden Globes data
* globes_visualizations folder - All visualizations created as jpg files

