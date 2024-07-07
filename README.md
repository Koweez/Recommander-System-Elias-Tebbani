# Movie Pairing Recommender System Project Report - Elias Tebbani

## Objective

## Dataset

For this project, I utilized two primary datasets:

- **MovieLens Dataset**: This dataset provides movie ratings and metadata, essential for understanding user preferences and movie characteristics.
- **IMDb Dataset**: Leveraged for additional movie metadata such as genres, titles, and ratings, enriching the information available for each movie.

## Tasks and Approach

## 1. Data Collection and Preprocessing

- **Data Integration**: Integrated data from MovieLens and IMDb datasets, focusing on movie metadata and ratings.
- **Data Cleaning**: Removed rows with missing genre information and adjusted data types for consistency.

## 2. Feature Engineering

- **Feature Extraction**: Extracted essential features such as genres, ratings, and start year for movies.
- **Data Merging**: Merged datasets based on movie titles (`primaryTitle`) to ensure comprehensive movie metadata.

### Incorporation of User Features

- **Attempted Integration**: Tried incorporating user features such as age, sex, etc., into the collaborative filtering model to enhance recommendation accuracy.
- **Challenges Faced**: Encountered difficulties in effectively incorporating user features due to matrix computation errors and lack of significant results.

### Bayesian Personalized Ranking (BPR) Model

- **Alternative Approach**: Explored the Bayesian Personalized Ranking model as an alternative to collaborative filtering.
- **Implementation Challenges**: Faced challenges in implenting the BPR specifically to the project problem.

## 3. Recommender System Development

- **User-Item Matrix**: Constructed a user-item interaction matrix from movie ratings data (`ratings_matrix_df`), crucial for collaborative filtering.
- **Collaborative Filtering**: Implemented collaborative filtering using TensorFlow to predict movie ratings and provide personalized recommendations based on user preferences.
- **Hyperparameter Tunning**: Different hyperparameters were tested to find the optimal values.

## 4. Algorithm Development

- **Recommendation Algorithm**: Developed an algorithm to suggest movies likely to be enjoyed together by couples, incorporating movie features such as genres and ratings using collaborative filtering

## 5. Evaluation

- **Model Evaluation**: Calculated the average of the difference between the original ratings and the predicted ratings.

## 6. 

### Conclusion

The project effectively utilized data integration, feature engineering, and TensorFlow-based collaborative filtering to develop a movie recommender system. While traditional matrix factorization (like SVD) wasn't explicitly implemented, the approach leveraged TensorFlow for predictive modeling based on user-item interactions and movie characteristics. This approach resulted in personalized movie recommendations, enhancing user engagement and satisfaction.

---

For detailed implementation code and further insights, please refer to the [GitHub repository](link-to-your-repo) associated with this project.
