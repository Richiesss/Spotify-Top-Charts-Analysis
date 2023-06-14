<h1 align="center"> 📈 2000-2019 Spotify Top Charts Analysis 📈 </h1>
This project runs analysis on an audio statistics dataset to understand the music trends and their transition over the past 2 decades.

<h2 align="center"> Dataset </h2>

[*Top Hits Spotify from 2000-2019*](https://www.kaggle.com/datasets/paradisejoy/top-hits-spotify-from-20002019) on Kaggle. This contains 20 columns of the top 100 tracks from each year during 2000-2019, therefore 2000 tracks total. Columns include but not limited to: artist name, track name, release year, tempo, duration, genre, and instrumentalness.

<h2 align="center"> Code </h2>

- [**Audio_Summary_Visualized.ipynb**](https://github.com/hina0830g/Spotify-Top-Charts-Analysis/blob/main/Audio_Summary_Visualized.ipynb) <br>
Reads the Kaggle dataset, cleans the data, and creates a new dataset (pandas dataframe). Lastly, it uses seaborn to create a 4-panel plot displaying the statistics of 4 parameters: tempo, duration, key, and genre.
- [**Time_Series_Analysis.ipynb**](https://github.com/hina0830g/Spotify-Top-Charts-Analysis/blob/main/Time_Series_Analysis.ipynb) <br>
Uses the [dataset](https://github.com/hina0830g/Spotify-Top-Charts-Analysis/blob/main/Top_Hits_2000_2019) created by Audio_Summary_Visualized.ipynb and calculates the mean tempo and duration and how many times each genre and key has appeared each year (2000~2019). 

- [**spotify.Rmd**](https://github.com/hina0830g/Spotify-Top-Charts-Analysis/blob/main/spotify.pdf) <br>
Shows five number summary, linear regression on duration & tempo. 
