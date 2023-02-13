# Prediciting Spotify's Top 100 Songs
The goal of this project is to build an algorithm that can predict within reason what kind of music will be on the Spotify pop charts next year. 

### Table of Contents
* [Data Exploration](#explore)
* [My Predictions](#predict)
* [Numerical Expectations](#expect)
* [Time Series Forecasting](#forecast)

## Data Exploration <a class="anchor" id="explore"></a>
An initial exploration of the [Kaggle](https://www.kaggle.com/datasets/muhmores/spotify-top-100-songs-of-20152019) dataset was conducted. Features were selected based on which were most accessible to measure and predict for the goal of this project. The features selected are defined in the table below and refined/engineered in the code. The descriptions were based on my interpretation, the author of the dataset and the [Spotify API](https://developer.spotify.com/documentation/web-api/reference/#/operations/get-several-audio-features). 

To learn more...
1. Click on "Spotify_data_exploration.ipynb" to see the code, or download and run it! :) 
2. Visit my [website](https://abrios.wixsite.com/thehub/my-blog/categories/spotify-analysis) for an in depth discussion of the exploration. 

| Feature | Description |
| --- | --- |
| year released | The number of years difference between the release year and the year the song was on the charts. |
| bpm | Song tempo measured in beats per minute. |
| nrgy | Energy is a measure from 0.0 to 1.0 and represents a perceptual measure of intensity and activity. |
| dnce | How easy it is to dance to the song on a scale from 0-1 (low to high). |
| dB | The loudness of the song and measured in (negative) decibels. |
| live | From 0-1, a high rating means the song was more likely recorded live. |
| val | A measure from 0.0 to 1.0 describing the musical positiveness (happy, upbeat) conveyed by a track. |
| dur | The duration of the song in seconds. |
| acous | A confidence measure from 0.0 to 1.0 of whether the track is acoustic. |
| spch | Speechiness detects the presence of spoken words in a track. |
| pop | Popularity of the song from 0-1, not a ranking. |

## My Predictions* <a class="anchor" id="predict"></a>
###### *This section of the README is based on my personal observations and opinons. "Numerical Expectations" is rooted in numerical predictions based on actual data trends. 

So here's the deal... I am expecting this experiment to fail. I'm actually trying to prove that the forecasting is inaccurate because mass media consumption trends changed with the introduction of the pandemic and TikTok. 

The data is between the years 2010-2019. The concept of viral sounds existed long before 2020-- if you're a millenial/gen z, you probably still quote Vines on the regular. However, the introduction of TikTok allowed for the capture of viral sounds independently from the videos they originated from. TikTok has an incredibly vast reach, having found its way into most other social/consumer medias, from reels on Instagram to Spotify generated playlists of the top songs on TikTok. The platform helped popularize more independent and 'throwback' music with mainstream consumers. As the mainstream continues to diversify, trends may become more difficult to predict because the data will continue to be more widespread. In tangent, this ties into the conversation that "genre" is a dying concept. Diversification of music means less ways to define boundaries across musics types. 

## Numerical Expectations <a class="anchor" id="expect"></a>
It is important to create an expected output because it will help us gauage if our actual forecasting output is reasonable. We are rooting our intuition in what we logically expect to happen. The table reflects our expectation that ~68% (1 std) of the forecasting algorithm output will fall in this range. 

![df_predictions](https://user-images.githubusercontent.com/111927463/218590450-c11a285f-622e-407c-9643-91cca4211164.png)

## Time series forecasting <a class="anchor" id="forecast"></a>
Coming soon...

A forecasting algorithm built with TensorFlow that predicts the features of next year's pop hits. 
