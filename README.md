# DAMG-6210---DMDD

Repo for the Music composer project

## Team members

|Member|  NUID| email | github username
|-------|--| -- | -- |
|      Ebenezer Ajay Williams | 002166250  | vincentsankeyraj.e@northeastern.edu | ebiskhan123
|      Abhinav Palem | 002791224  | palem.a@northeastern.edu | abhinav250997
## Database description
The Database comprises of 3 tables 
- The Spotify - All Time Top 2000s Mega Dataset  (https://www.kaggle.com/datasets/iamsumat/spotify-top-2000s-mega-dataset)
- The Artist Table - To be populated using the Spotify API
- The Song Table - To be populated using the Spotify API

The Spotify table comprises of following fields:
 - Index
 - Song Title
 - Artist
 - Top Genre
 - Year
 - Beats per minute (BPM)
 - Energy
 - Danceability
 - Loudness(dB)
 - Liveness
 - Valence
 - Length
 - Acousticness
 - Speechiness
 - Popularity
 
 The Artist table comprises of following fields:
 - Artist 
 - Popularity
 - Artist ID
 - Followers
 - Genre
 
 The Song table comprises of following fields:
 - Title
 - Album
 - Duration
 - ID

## Problem statement
As a music composer, I wish to know how popular my composition would be before i start composing the tune. Before composing any music I would pre determine the beats, Valence, loudness and other settings to compose the tune. I need to know the probable popularity of my song if i provide the rhythm settings as input. Additionally, if i wish to make a song in a particular genre, in a particular style, I wish to know the best artist to look at for inspiration. I also wish to know the best songs similar to the rhythm I wish to compose in to listen to.
Additionally, If i select a genre and the ideal popularity, I wish to know the best possible parameters to set for the rhythm. As a composer I also wish to know the best possible parameters to set for my rhythm if i provide the genre and the expected popularity.

## Proposed solution 
Use the Spotify Dataset table to perform regression and obtain the probable popularity of the song. 
Use the Spotify API to populate the Artist and Song tables. 
Use the date in the Spotify Dataset table and find the most similar Song Artist using distance metrics such as cosine similarity.
Use the Spotify Dataset table to find the closest popularity with that particular genre and provide the output metrics

## Project Scope:
 - Create an Artist table by using Spotify API
 - Create a Song table by using Spotify API
 - Music composer will have to set Beats per minute (BPM) , Energy, Danceability,     Loudness(dB, Liveness, Valence, Length, Acousticness, Speechiness and select the Genre of the song before composing to know the popularity and followers.
 - Music composers can know the dynamics of a song like Beats per minute, Energy, Danceability, Loudness(dB, Liveness, Valence, Length, Acousticness and by selecting the popularity and Genre in order to have maximum followers.