# MusicGenreClassification
Model to predict genre of a song

**Project Report:** [Report](https://github.com/mikecrist/MusicGenreClassification/blob/main/Report/Report_Music%20Genre%20Classification.pdf)

## Credits
This project was created for the Georgia Tech Master of Analytics program.<br>

**Course:** Data Mining and Statistical Learning (ISYE7406)<br>
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
![image](https://github.com/mikecrist/OpioidAbuseAnalysis/assets/31662579/af22390d-7379-42ad-9f78-8ebcc47fd2c3)
<p align="center">
Results Summary
</p>

The best performing model was the KNN model, which obtained an accuracy of 99.13%. The optimal k-value was determined by evaluating the cross-validation error for many values of k. This model should be used to predict opioid misuse in individuals so that healthcare professionals may take the necessary steps to avoid dangerous outcomes.

The KNN model was clearly the best performing model because it performed best on all metrics. However, selecting the second and third best models becomes more interesting, because accuracy / total error is not necessarily the most important metric to use for evaluation. The objective of the model is to predict whether an individual will misuse opioids, which is very dangerous for the individual and can result in overdose or death. For this reason, sensitivity is the most important metric, because this is the “true positive rate”, meaning the percentage of cases of opioid misuse that were correctly classified. It is more dangerous for the model to miss a case of opioid misuse (type II error) than it is for the model to incorrectly predict opioid misuse (type I error). The three best-performing models, ranked by sensitivity, are:
1. KNN (sensitivity 94.97%)
2. Naïve Baes (sensitivity 48.30%)
3. QDA (sensitivity 46.31%)

In addition to evaluating model performance, I also evaluated factor importance to determine the factors that had the greatest impact on the odds of opioid misuse. The five factors that most impact odds of opioid misuse are summarized below:
1. **Age:** We expect an 89-92% decrease in odds of opioid misuse if a person’s age is >= 50 (versus baseline of age 12-17), holding all other factors constant.
2. **Marital Status:** We expect a 35-48% decrease in odds of opioid misuse if a person is unmarried (versus baseline of divorced), holding all other factors constant.
3. **Hallucinogen Use:** We expect a 58-64% increase in odds of opioid misuse for each unit increase in hallucinogen use on the Likert scale, holding all other factors constant.
4. **Amphetamine Use:** We expect a 47-56% increase in odds of opioid misuse for each unit increase in amphetamine use on the Likert scale, holding all other factors constant.
5. **Ever Used Heroin:** We expect a 45-102% increase in odds of opioid misuse if a person has ever used heroin, holding all other factors constant.

***Policy Proposals***

Based upon the results of this project, the policy actions below would reduce opioid misuse in the US:
1. Educate students on the dangers of opioid misuse, beginning in elementary school. Continue education throughout high school.
    - Opioid misuse is more likely in younger age categories, so education must start early.
2. Incentive programs to reduce use of all illicit drugs.
    - Use of illicit drugs is a clear risk factor for opioid misuse. Offer incentive programs to encourage drug users to reduce or eliminate illicit drug use.
3. Offer marriage counseling to reduce divorce rate in the US.
    - Divorce is a clear risk factor for opioid misuse. Cultivating healthy marital relationships would reduce risk of opioid misuse.
4. Regular screening of patients.
    - Healthcare providers should request patients to complete the survey used to obtain the dataset for this project. Survey results can be entered into the KNN model to predict whether the patient will misuse opioids. If the model predicts opioid misuse, healthcare providers may decide against opioid prescription, or further educate the patient on responsible opioid use.


## Dataset
The dataset I used for this project can be found [here](https://github.com/mikecrist/MusicGenreClassification/blob/main/Data/archive%20(1)/music_genre.csv).

The dataset contains a set of audio features, provided by Spotify, for a large sampling of songs. Each row corresponds to a song, and each column corresponds to a feature of the song. One of the columns is the target variable, which is genre. There are 10 total genres provided in the dataset. The feature columns contain various attributes such as artist, song title, duration, key, tempo, loudness, etc. The total size of the dataset is 7.5MB; it contains 50K rows and 18 columns. 

## Citations
Bhardwaj, Ashutosh. “Silhouette Coefficient : Validating Clustering Techniques.” *Towards Data Science*, 27 May 2020, https://towardsdatascience.com/silhouette-coefficient-validating-clustering-techniques-e976bb81d10c.

Blaufuks, William. “FAMD: How to Generalize PCA to Categorical and Numerical Data.” *Towards Data Science*, 28 Mar. 2022, https://towardsdatascience.com/famd-how-to-generalize-pca-to-categorical-and-numerical-data-2ddbeb2b9210.

Bonthu, Harika. “KModes Clustering Algorithm for Categorical Data.” *Analytics Vidhya*, 13 June 2021, https://www.analyticsvidhya.com/blog/2021/06/kmodes-clustering-algorithm-for-categorical-data/.

Chaudhary, Shivam. “Why ‘1.5’ in IQR Method of Outlier Detection?” Medium, *Towards Data Science*, 26 Aug. 2020, https://towardsdatascience.com/why-1-5-in-iqr-method-of-outlier-detection-5d07fdc82097.

Yassin, Diana. “A Brief History of Streaming Services.” *The Michigan Daily*, 5 Dec. 2019, https://www.michigandaily.com/music/brief-history-steaming-services/.

