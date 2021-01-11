# BrainStation-Capstone

**Overview of the Project:**

What I wanted to do with this project is to both be able to do the Spotify RecSys challenge as well as build my own recommender system to see what new artist that I could add to my own personal spotify playlist. The data consists of 1 million unique spotify playlists that includes over 2 million unique songs as well as nearly 300 thousand artists. Unfortunately, the data cannot be distributed publicly. However, it is open to the public if you decided to join the open competition on AICrowd. In order to utilize the surprise library to build a recommender system, I had to create a ranking system. I based it on 2 factors. The first was to count how many times an artist appeared in a playlist, that would serve as the baseline. The second factor was to add a weighting to that baseline. The weighting would depend on how many unique artists were in that playlist. The more artists within the playlist the lower the weighting would be. This ranking system now allows me to create a collaborative filtering algorithm with the help of the surprise library. 

** Tools Used:**
Surprise and scikit-learn are the main machine learning libraries used along with the standard pandas and numpy

** Files: **

1.`Dataframe_capstone_final_outputcleared` - Exploration and Data Analysis of the dataset given as well as initial model testing to see which algorithm in surprise would be best suited for the final model to be based on. After deciding on SVD, did GridSearch to help optimize the parameters.

2. `Capstone Model` - Final model prototype that only uses 1 thousand of the 1 million playlists. Did evaluation based on my own music taste.

3. `Capstone Model Test` - Created a new evaluation that has no bias. Removed existing artists from certain playlist to see if the recommender system could re-recommend the artists that had been removed.

Link to competition: https://www.aicrowd.com/challenges/spotify-million-playlist-dataset-challenge
