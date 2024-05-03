# Movie Recommendation System
<img src="https://www.freecodecamp.org/news/content/images/size/w1000/2023/11/movie-recommendation.png" alt="Movie Recommendation System" width="1000px" height="250px">

This project is a movie recommendation system that utilizes various filtering techniques to provide personalized movie recommendations to users. The system plays a crucial role in enhancing user experience and engagement on movie streaming platforms by helping users discover new movies tailored to their preferences.

## About the Filtering Techniques

### Collaborative Filtering
Collaborative Filtering identifies patterns in user behavior and recommends movies based on the preferences of users with similar tastes. For this, we utilize the [Surprise](http://surpriselib.com/) library, a Python scikit for building and analyzing recommender systems. The specific modules used for collaborative filtering are:

- Dataset from Surprise: A module to load a dataset.
- Reader from Surprise: A module to define the format of the input file.
- SVD (Singular Value Decomposition) from Surprise: A collaborative filtering algorithm based on matrix factorization.
- model_selection from Surprise: A module providing tools for model selection and evaluation.

### Popularity-Based Filtering
Popularity-based filtering recommends movies based on their popularity among users. The formula used to calculate popularity-weighted ratings (WR) is:
WR = (v / (v + m)) * R + (m / (v + m)) * C
Where:
- v is the number of votes for a movie,
- m is the minimum number of votes required,
- R is the average rating of the movie, and
- C is the average rating across all movies.

### Content-Based Filtering
Content-based filtering recommends movies based on their features and similarities. We use a similarity matrix to get a list of similar movies based on the cosine similarity between movie vectors.

### Hybrid-Based Filtering
Hybrid-based filtering combines content-based and collaborative filtering techniques. It leverages a combination of content-based filtering, which analyzes item features, and collaborative filtering, which analyzes user behavior, to provide more accurate and diverse recommendations.

## Dataset
The dataset used for training and testing the recommendation system can be found at the following link:
[Dataset Link](https://drive.google.com/file/d/1hmK2Vej7YfLMW7OemdqPBUQcIdksTGr3/view)

## Project Report
For a detailed report on the "Recommendation Filtering Techniques", please refer to the report available [here](https://github.com/vn33/Movie-Recommendation-System/blob/master/Recommendation%20system%20report_VishalNaik.pdf).

