# Song Popularity Classification and Content Based Recommendation System
by Allison Ward

## Project Overview
Wavelengths is a new music streaming company seeking to introduce listeners to the best possible listening experience. They are seeking help in creating a classification system for new music for their listeners based on music popularity. Recommending songs that are popular will likely increase listening time.
 Additionally, a recommendation system using content-based filtering is established to suggest new songs based on feature similarity.  This provides the listener with a seamless  experience and can also open them up to new artists or songs they have never heard before.
 For a streaming service, these are essential ways to keep listeners on their app and enjoying the songs they love. Increased streaming time will likely increase revenue and customer buy-in for the service, which is essential in today’s competitive market. 

## Data Overview

The dataset is from https://www.kaggle.com/datasets/vatsalmavani/spotify-dataset. It includes 170,653 Spotify songs, each with quantified audio features such as valence, energy, danceability, tempo, as well as song information such as duration and year released. Songs range from all genres, spanning release years between 1921 to 2020. While the data analyzes Spotify song features, Wavelengths will be able to analyze trends in the data to implement in their own service. 
Limitations of the data include that this is not an official Spotify dataset. In particular, the “popularity” feature might be biased. Further investigation into “popularity”, including more concrete data such as number of streams of playlist adds, would benefit a future analysis. 


## Exploratory Data Analysis
Images here

## Modeling - Classification Based on Popularity

“Popularity” was the metric used for classification, which ranges from 0 to 100. While other features were included in the official Spotify API, there was no explanation of popularity. It is assumed that a higher popularity is representative of more popular songs, with lower popularity representative of less popular songs. There was an unusual amount of 0’s in the data (16%), which upon further inspection is likely because 0 is representative of a null value. Therefore, zeroes were removed, leaving a bell curve of popularity. 
“Popular” songs were those categorized with a popularity of 50-100, with unpopular songs categorized as those with a rating of 0-50. 

## Content-Based Filtering using Nearest Neighbors

Individual user data was not available, only song features and general popularity. Therefore, the best method to achieve a recommendation system was utilizing content-based filtering, which compares the quality of two items (in this case, songs) and measures the distance between them. The first recommendation system used cosine distance as the method for calculating distance.


## Business Recommendations & Insights

## Future Steps

## Sources

