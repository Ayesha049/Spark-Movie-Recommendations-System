# Spark-Movie-Recommendations-System
The movie recommendation system aims to selectively predict and suggest films that a specific user is most likely to be interested in watching. Our project utilizes clustering algorithms for movie recommendations, a system that forecasts user preferences based on their past movie-watching history or activity. The recommendation process begins by extracting features from the Movielens Dataset and subsequently employing clustering algorithms, including K-Means clustering, Gaussian Mixture Model, and Latent Dirichlet Allocation Model, to form movie clusters. Subsequently, we identify the user’s last highest rated movie, determine its cluster, and present the top ten highest and most-rated movies from that cluster as recommendations. The evaluation metric for the clustering algorithms is the silhouette coefficient, with results indicating that K-Means clustering yields superior clusters compared to other algorithms.

## Dataset 
In this project, used the Movielens dataset for the movie recommendation system. GroupLens Research has collected Rating data of movies from users over periods of time and made them available in the MovieLens website.The movielens latest dataset were created by 330975 users between January 09, 1995 and July 20, 2023. This dataset was generated on July 20, 2023 and it contains 33832162 ratings and 2328315 tag applications across 86537 movies. The dataset contains the following files: genome-scores.csv, genome-tags.csv, links.csv, movies.csv, ratings.csv, tags.csv. This project mostly utilises data from ratings.csv for extracting the features populartiy and average rating of a specific movie, and data from movies.csv for extracting the feature genre and movie specific metadata.

## workflow
- We loaded the move lens dataset for training Apache Spark
- We trained our K means model with movie lens dataset
- We tuned the model hyper parameters
- We implemented LDA and GMM clustering algorithms and train the models
- We compared the performance of K means, LDA and GMM algorithms

## Final Outcome
We filtered users' top ten latest-rated movies, selected the highest-rated among them, and identified its cluster. Based on this cluster, we provided personalized recommendations by presenting the top ten movies with the highest average ratings and user counts. We employed three clustering algorithms: K-Means, Gaussian Mixture Model, and Latent Dirichlet Allocation (LDA). Our findings indicated that K-Means produced better clusters compared to the others, despite LDA being faster. Future work will explore combining results from different clustering methods and experimenting with various feature selection models for improved recommendations.

