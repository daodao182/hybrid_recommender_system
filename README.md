# Hybrid Recommender System

# Item- based content filtering
#### content-based filtering focuses on the similarities in feactures(movie in this case) of the specific user, provide recommendations based the the user's ratings on the movies he has seen.
# User-based Collaborative filteirng
#### user-based Collaborative filteirng relies on the preference of similar users,provide recommendations based on the similar user's data.

# Dataset
## MovieLens20M dataset.
#### 20M ratings.csv and 27K movies.csv
#### merging two dataframe using common unique id(movieid).

## Functions
#### Correlation between users
#### Weighted rating = Correlation * user rating

# Steps:
#### Data Preparation
#### Random user analysis
#### Comparing with other users watching the same movies and identifying the most similar user
#### Calculating weighted average recommendation
#### printing user based and item based recommendation


# parameters 

# We could not upload the rating csv file in github
    # File too large for github repo
    Refs:
    #https://www.kaggle.com/code/mustafayurtcan/movielens-hybridrecommendersystem
    #https://www.kaggle.com/code/mfaaris/hybrid-and-tensorflow-recommender-system
    #https://www.kaggle.com/code/bhu1111/movies-recommendation-system
