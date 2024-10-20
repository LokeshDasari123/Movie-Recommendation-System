# Movie Recommendation System

This project implements a movie recommendation system using Python and Streamlit. The backend processes movie data and generates recommendations based on user-selected movies.

## Overview

1. *Run Main.ipynb*: This Jupyter Notebook prepares the movie dataset and creates the necessary pickle files (movies_list.pkl and similarity.pkl) for movie recommendations.
   
2. *Run app.py*: This script launches a Streamlit application, which provides an interactive interface for users to select a movie and receive recommendations.

### Movie Recommendation Logic

- The dataset is loaded, and movie tags (overview and genre) are combined.
- A CountVectorizer is used to convert text data into a matrix of token counts.
- Cosine similarity is calculated to find similar movies based on the combined tags.
- The user can select a movie, and the top 5 recommended movies will be displayed along with their posters.

## Required Libraries

Make sure to install the following libraries:

```bash
pip install pandas
pip install streamlit
pip install scikit-learn
pip install requests

To run use this command:
streamlit run app.py
