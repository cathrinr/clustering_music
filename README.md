# Clustering music with KMeans

### Note
Some of the code uses the Spotify Developer API: If you don't already have one, create a Spotify developer account to get your own credentials. 


## Data Preparation and Feature Selection
Given a dataset of about 5000 songs available on Spotify, the task is to create an arbitrary number of playlists. You can use the 13 features that come with the Spotify data. The data set does not require much cleaning. It is only necessary to drop the 'type' column, as it contains only NaN, and to drop duplicates. 
Based on my knowledge of music, I decided not to consider the following three columns, since they do not affect the human perception of music very much: Key, Duration and Time Signature. Based on correlation and variance, the feature energy was also dropped. 

## Choosing a number of clusters
To decide on a reasonable number of clusters, I took into account two different considerations: Inertia and Silhouette Score as technical indicators, and answers to my question "What makes a playlist a good playlist?", where an important factor is the total length and number of tracks. In the end, I decided on 25 playlists. 

## Insights into the clusters
To better understand the composition of the clusters, I decided to gather additional information from the Spotify API. I attached each artist's genre to each song and plotted word clouds. This visualization allows for easy access to the type of music. 

## Listen to your playlists on Spotify
As an add-on I also implemented the option to send the newly created playlists directly to Spotify, so you can listen to them. 

Have fun with this project! 





