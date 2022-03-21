# Group 71

**Group Members**:
* Lance Te
* Thomas Mansfield
* Ava Gardiner
* Darcey Burch

## Summary

### Our Goal
Our goal is to determine the key factors that make a hit song. In order to address the core question, we will investigate the following questions:
* What attributes should a song have to be successful?
* Is it possible for a song that sounds sadder or angry to become a hit?
* Does the artist influence the popularity of a song?
* Does the song need to be in a certain genre to be a hit?
* Does a collaboration gain more popularity to a song that has a single artist?


### The Data
The data we use is obtained from Spotify's Web API. To access this web API, we created a Spotify Developer Account (https://developer.spotify.com), set up an application and accessed the API through the Spotipy package.


### Analysis
We plan to use the following techniques in our analysis:
* **Linear regression:** The popularity value of a track is a score between 0-100. With explanatory variables such as energy, danceability, and liveness, we will use linear regression to predict this popularity value.
* **Clustering:** Clustering will allow us to group together songs with similar features, and help us recognise patterns in popular music tracks.
* **Heat Map:** Heat maps will be used to identify which features of a set of popular tracks tend to be high or low.

## Use
When you create an account for Spotify's API, they will provide a CID and secret. You will need to create a `.env` file with these values:
```py
cid = {cid};
secret = {secret};
```

## Column Descriptions
| Name | Description
| :--- | :----------
| artist_name | Unique identifier for each track
| track_name | Name of the track
| popularity | A score between [0-100] measuring an artist's popularity
| year | The year in which the track was released
| danceability | A score between [0.0-1.0] measuring how suitable a track is for dancing
| energy | A score between [0.0-1.0] measuring a track's intensity and activity
| key | The estimated overall key of the track
| loudness | The overall loudness of a track in decibels (dB)
| mode | Indicates the modality (major or minor) of a track
| speechiness | Detects the presence of spoken words in a track
| acousticness | A score between [0.0-1.0] measuring whether the track is acoustic
| instrumentalness | Predicts whether a track contains no vocals
| liveness | Detects the presence of an audience in the recording
| valence | A score between [0.0-1.0] measuring the musical positiveness conveyed by a track
| tempo | The overall tempo of a track in beats per minute (BPM)
| duration_ms | Duration of a track in milliseconds (ms)
| time_signature | The estimated overall time signature of a track

