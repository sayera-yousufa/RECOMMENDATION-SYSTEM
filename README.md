# RECOMMENDATION-SYSTEM

*COMPANY*: CODTECH IT SOLUTIONS

*NAME*: SAYERA YOUSUFA

*INTERN ID*: CT04DK237

*DOMAIN*: MACHINE LEARNING

*DURATION*: 4 WEEKS

*MENTOR*: NEELA SANTOSH


## Project Title
**Content-Based Movie Recommendation System**

## Project Description

This project implements a **content-based movie recommendation system** using text processing and similarity measures. It recommends movies similar to a given movie based on their genres and plot summaries (overview). The system leverages natural language processing (NLP) techniques to vectorize movie metadata and computes cosine similarity to find the most similar movies.

---

## Dataset

The dataset used (`Movie_dataset.csv`) contains various features related to movies, such as:
- `id`: Unique identifier for each movie
- `title`: Movie title
- `genre`: Genres of the movie (e.g., Drama, Crime)
- `overview`: Plot summary of the movie
- `original_language`: Language of the movie
- `popularity`: Popularity score
- `release_date`: Release date of the movie
- `vote_average`: Average rating
- `vote_count`: Number of votes

A `tags` column is created by combining `genre` and `overview` for text processing.

---

## Technologies Used

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Scikit-learn (CountVectorizer, cosine_similarity)

---

## Model Details

- **Approach**: Content-based filtering
- **Text Processing**: Used `CountVectorizer` to convert movie `tags` into a matrix of token counts (max 10,000 features, English stop words removed)
- **Similarity Measure**: Cosine similarity between vectorized movie tags
- **Recommendation Logic**: For a given movie, the system computes similarity scores with all other movies and returns the top 5 most similar movies (excluding the input movie itself in improved versions)

---
### Prerequisites

Ensure you have Python installed along with the following libraries:  
`pandas`, `numpy`, `scikit-learn`

## Results

The recommendation system successfully suggests movies based on their content similarity. Key observations:

- **Example Output**: For "The Shawshank Redemption", the system recommended movies like "Anything for Her", "The Woodsman", "The Getaway", and "Pusher II", which share similar themes (e.g., drama, crime, imprisonment).

<img width="830" alt="Image" src="https://github.com/user-attachments/assets/6b2b3b48-42ec-46c6-aae4-09ffe4844d61" />

- **Performance**: The system is efficient for small to medium datasets.
The system demonstrates a practical approach to recommending movies based on textual metadata, making it useful for movie streaming platforms or personal movie discovery tools.

## Acknowledgements

This project was completed as part of my internship at **CodTech IT Solutions**.
```
