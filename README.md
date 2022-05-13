# Spotify_Playlist_Clustering
This project is done as a part of my Machine Learning Theory Assignment where we have 
to apply a Machine Learning Technique for the project.

# Project Description

Music is one of the universal cultural aspects of all human societies. People listen to various kind of music to show emotions, feelings and communicate
and groove to the music of their interest.If you want to keep your brain engaged throughout the aging process, listening to or playing music is a great tool.
It provides a total brain workout. Research has shown that listening to music can reduce anxiety, blood pressure, and pain as well as improve sleep quality, mood, mental alertness, and memory.

[Spotify](https://www.spotify.com) is the most popular global audio streaming service with 365m users, including 165m subscribers across 178 markets.
<p align="center" >
  <img src="https://developer.spotify.com/assets/branding-guidelines/logo@2x.png" >
</p>

# Data Extraction
<ul> Steps:
  <li> Create an account on https://developer.spotify.com/dashboard/</li>
  <li> Import the Spotipy module using pip</li>
  <li> Click on Create an app option, which will create a client id and client secret which is important for getting authorization</li>
  <li> Get the playlist id which we want to retrieve, in our case it is https://open.spotify.com/playlist/7xNEW3kVH1KXZ3yevHz5u4</li>
  <li> Retrieve the audio features of the song into a csv file. Follow the jupyter notebook for extracting the playlist data</li>
</ul>

#Model 
<p> In this project,we are going to take a playlist and divide the songs based on audio features into clusters 
  where similar songs fall in the same cluster. For this we are using <b>KMEANS algorithm</b> to find the number of clusters
  and cluster the songs. Then we performed <b>PCA analysis</b> to check if the information could be preserved as we reduce the dimensionality.
  Then we performed <b>Smote analysis</b> to balance the data by oversampling the minority class. Finally we applied various classifiers like
  <b> SVM (linear, polynomial and RBF), Random Forest, Decision Tree, KNN , Naive Bayes</b> to predict the cluster for a new data point.
    After training the model and fitting it on the trained data we found out that<b> SVM with polynomial kernel </b>prrovides the best accuracy
  when it comes to making predicitions. with an accuracy of <b>98.3%</b>.
 </p>
