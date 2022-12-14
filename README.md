# Hybrid Recommender System

# content filtering
#### content-based filtering focuses on the similarities in feactures(movie in this case) of the specific user, provide recommendations based the the user's ratings on the movies he has seen.

# User-based Collaborative filteirng
#### user-based Collaborative filteirng relies on the preference of similar users,provide recommendations based on the similar user's data.(target users and other users)
# Item-based Collaborative filtering
#### In item-based collaborative filtering we focus on the items rather than the users(items that target user interacts with and other items).

#### We used user-based and item-based collaborative filtering method to make a hybrid recommendation system

# Dataset
#### MovieLens20M dataset.
#### tmdb_movies 7M dataset
#### 20M ratings.csv and 27K movies.csv
#### merging two dataframe using common unique id(movieid).

## Functions
#### Correlation between users
``` final_df.T.corr()```
#### Correlation for item based
```user_movie_df.corrwith(movie_name)```

#### Weighted rating 

```top_users_ratings["weighted_rating"] = top_users_ratings["correlation"] * top_users_ratings["rating"]```
```agg({"weighted_rating": "mean"})  ``` 

# Steps:
#### Data Preparation
#### Random user analysis
#### Comparing with other users watching the same movies and identifying the most similar user
#### Calculating weighted average recommendation
#### printing user based and item based recommendation


# Weighted rating
#### W=(R*v+C*m)/(v+m)
#### W: weighted-rating
#### R: average(mean) of the ratings of movie from number 1 to number 10
#### v:  number of votes for the movie
#### m: minimum votes required to be listed in Top 250


# We could not upload the rating csv file in github
    # File too large for github repo
    Refs:
    #https://www.kaggle.com/code/mustafayurtcan/movielens-hybridrecommendersystem
    #https://www.kaggle.com/code/mfaaris/hybrid-and-tensorflow-recommender-system
    #https://www.kaggle.com/code/bhu1111/movies-recommendation-system
