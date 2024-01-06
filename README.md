# MusicGenreClassification
In this project I built, evaluated, and analyzed a variety of classification models to obtain the best performing model for predicting genre of a song.

**Project Report:** [Report](https://github.com/mikecrist/MusicGenreClassification/blob/main/Report/Report_Music%20Genre%20Classification.pdf)

## Credits
This project was created for the Georgia Tech Master of Analytics program.<br>

**Course:** Computational Data Analysis (ISYE6740)<br>
**Team:** Michael Crist

## Table of Contents
- [Abstract](#Abstract)
- [Conclusions](#Conclusions)
- [Dataset](#Dataset)
- [Citations](#Citations)

## Abstract
Complete report [here](https://github.com/mikecrist/MusicGenreClassification/blob/main/Report/Report_Music%20Genre%20Classification.pdf).

Beginning with Napster in 1999, online music streaming services have gained popularity with astounding speed. The introduction of Napster directly caused the first ever global decrease in album sales, as a new technology disrupted an age-old industry (Yassin, 2019). By the mid-2010s, most music listeners, globally, utilized one streaming platform or another for their music consumption. Spotify has established itself as one of the most popular streaming services. One of the most important services that Spotify offers (as well as most other streaming platforms) is the curation of playlists and song recommendations for its listeners. The goal of this project is to classify the genre of a song, given input feature data for a particular song. This provides value by automating the process of classifying song genre, thus allowing for automatic playlist creation and song recommendation based upon a listener’s preferred genre.

## Conclusions


## Dataset
The dataset I used for this project can be found [here](https://github.com/mikecrist/MusicGenreClassification/blob/main/Data/archive%20(1)/music_genre.csv).

The dataset contains a set of audio features, provided by Spotify, for a large sampling of songs. Each row corresponds to a song, and each column corresponds to a feature of the song. One of the columns is the target variable, which is genre. There are 10 total genres provided in the dataset. The feature columns contain various attributes such as artist, song title, duration, key, tempo, loudness, etc. The total size of the dataset is 7.5MB; it contains 50K rows and 18 columns. 

## Citations
Bhardwaj, Ashutosh. “Silhouette Coefficient : Validating Clustering Techniques.” *Towards Data Science*, 27 May 2020, https://towardsdatascience.com/silhouette-coefficient-validating-clustering-techniques-e976bb81d10c.

Blaufuks, William. “FAMD: How to Generalize PCA to Categorical and Numerical Data.” *Towards Data Science*, 28 Mar. 2022, https://towardsdatascience.com/famd-how-to-generalize-pca-to-categorical-and-numerical-data-2ddbeb2b9210.

Bonthu, Harika. “KModes Clustering Algorithm for Categorical Data.” *Analytics Vidhya*, 13 June 2021, https://www.analyticsvidhya.com/blog/2021/06/kmodes-clustering-algorithm-for-categorical-data/.

Chaudhary, Shivam. “Why ‘1.5’ in IQR Method of Outlier Detection?” Medium, *Towards Data Science*, 26 Aug. 2020, https://towardsdatascience.com/why-1-5-in-iqr-method-of-outlier-detection-5d07fdc82097.

Yassin, Diana. “A Brief History of Streaming Services.” *The Michigan Daily*, 5 Dec. 2019, https://www.michigandaily.com/music/brief-history-steaming-services/.

