# Song Recommender Project 
Idea is to recommend a similar song to the song entered by the user. 
If a song is in the top 100 billboard charts the song recommended will be another 'hot' song from this list. 
If not then the song recommended will be one of similar musical features.

To get the list of popular songs I scraped the 'hot-100' song list from the billboard website (Billboard_Top_100.ipynb).

Next I collected as many random songs from Spotify as I could.
I did this by importing a small playlist and getting the musical features of every song from every album that each artist in the playlist had produced (Spotify_Collect_Data.ipynb).

I then divided all the obtained songs into clusters based on their musical features using a K means clustering model (Clustering.ipynb).

The final demo combines these files and takes an input song, classifies it into a cluster and recommends another song from the same cluster in my collected dataframe (Song_Recommender_Demo.ipynb).

