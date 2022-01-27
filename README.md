



# Escape the bubble! 
## A trade-off between personalization and diversity in movie recommendations

<br>

### This capstone project is the graduation work of four students of the Neue-Fische Bootcamp in Data Science, between September and December 2021. 

<br>

## Project description:

Recommender systems are both a blessing and a curse. On the one hand, they provide the user with recommendations, tailored to his/her personal profile. On the other hand, the user is at risk of getting stuck in a personalized filter bubble.
A filter bubble gradually isolates a user by decreasing the diversity of recommendations.
Common recommender engines are content-based and collaborative filtering. While content-based filtering suggests recommendations based only on the similarity of items, collaborative filtering takes user ratings into account. Depending on the information the users have given so far, these recommendations may still be of little variation. 
In this project, we developed a recommender engine that produces personalized recommendations for movies. Further, we implemented an algorithm which gives the user the choice, how far he/she wants to leave the filter bubble. With this increased diversity, we provide a better experience for the user.



## Project team:
- Alexandra Zimmermann-Rösner, Dipl.- Biologist, [GitHub](https://github.com/AlexaZiRo/)
- Hassan Mohamed, MSc., Physicist, [GitHub](https://github.com/flux511/)
- Konstanze Braun, MSc., Psychologist, [GitHub](https://github.com/konni-b/)
- Jana Conradi, MSc.,  Bio Scientist, [GitHub](https://github.com/JanaConradi/) 



<br>


<br> 

## Graduate Presentation: [pdf](https://github.com/flux511/recommender-system-capstone/blob/main/presentation/Escape_the_bubble_presentation.pdf), [YouTube_video](https://www.youtube.com/watch?v=U-Fmn2jkK7w&t=834s),[Dashboard](https://dashboard-movie.herokuapp.com/)

<br>

## Data

To build the movie recommendations, following datasets were used:
+ Dataset from MovieLens<br>
Small: 100,000 ratings and 3,600 tag applications applied to 9,000 movies by 600 users. Last updated 9/2018. Provided by the University of Minnesota<br>
[Link](https://grouplens.org/datasets/movielens/)
+ TMDB movie metadata, uploaded on Kaggle<br>
[Link](https://www.kaggle.com/rounakbanik/movie-recommender-systems/data)

<br>

## The main project notebooks:
- [EDA_users](https://github.com/flux511/recommender-system-capstone/blob/main/notebooks/1_EDA_Users.ipynb) and [EDA_movies](https://github.com/flux511/recommender-system-capstone/blob/main/notebooks/1_EDA_Movies.ipynb)
- [Collaborative filtering recommendations](https://github.com/flux511/recommender-system-capstone/blob/main/notebooks/6_top_n_recommendations.ipynb)
- [Diversity optimization](https://github.com/flux511/recommender-system-capstone/blob/main/notebooks/9b_optimizing_diversity.ipynb) 
- [Dashboard](https://github.com/flux511/recommender-system-capstone/blob/main/notebooks/8b_Dashboard.ipynb)  

<br>

## Requirements
pyenv with Python: 3.9.4

### Installation with PIP
### Surprise Library

pip install scikit-surprise
<br>

### NLTK
pip install nltk<br>


<br>
### Pandas-Profiling
pip install -U pandas-profiling[notebook]<br>
jupyter nbextension enable --py widgetsnbextension
<br>

## Environment
```BASH
make setup 

#or 

pyenv local 3.9.4
python -m venv .venv
pip install --upgrade pip
pip install -r requirements.txt
source .venv/bin/activate
```
### The general flowchart of the project can be illustrated in this diagram:
<br>

![Alt text](./images/recsys_flowchart.png?raw=true "Title")