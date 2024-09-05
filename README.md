# Content-Based-Movie-Recommender-System-with-sentiment-analysis-using-AJAX
![Static Badge](https://img.shields.io/badge/Python-3.8-blue)
![Static Badge](https://img.shields.io/badge/Framwork-Flask-red)
![Static Badge](https://img.shields.io/badge/Frontend-HTML%2FCSS%2FJS-Purple)
![Static Badge](https://img.shields.io/badge/API-TMBD-yellow)

Content Based Recommender System recommends movies similar to the movie user likes and analyses the sentiments on the reviews given by the user for that movie.
<br>
<br>
The details of the movies(title, genre, runtime, rating, poster, etc) are fetched using an API by TMDB, 
https://www.themoviedb.org/documentation/api, and using the IMDB id of the movie in the API, I did web scraping to get the 
reviews given by the user in the IMDB site using beautifulsoup4 and performed sentiment analysis on those reviews.
<br>
# How to get the API key?
Create an account in https://www.themoviedb.org/, click on the API link from the left hand sidebar in your account settings and 
fill all the details to apply for API key. If you are asked for the website URL, just give "NA" if you don't have one. You will see the
API key in your API sidebar once your request is approved.
<br>
# How to run the project?
1. Clone or download this repository to your local machine.
2. Install all the libraries mentioned in the requirements.txt file with the command pip install -r requirements.txt
3. Get your API key from https://www.themoviedb.org/. (Refer the above section on how to get the API key)
4. Replace YOUR_API_KEY in both the places (line no. 15 and 29) of static/recommend.js file and hit save.
5. Open your terminal/command prompt from your project directory and run the file main.py by executing the command python main.py.
6. Go to your browser and type http://127.0.0.1:5000/ in the address bar.
7. Hurray! That's it.

# Architecture:
![Screenshot (17)](https://github.com/user-attachments/assets/b29c48ee-3757-4f9b-b980-f7805cc07fd6)


# Similarity Score :
How does it decide which item is most similar to the item user likes? Here come the similarity scores.
<br>
<br>
It is a numerical value ranges between zero to one which helps to determine how much two items are similar to each other on a scale of zero to one. This similarity score is obtained measuring the similarity between the text details of both of the items. So, similarity score is the measure of similarity between given text details of two items. This can be done by cosine-similarity.

# How Cosine Similarity works?
Cosine similarity is a metric used to measure how similar the documents are irrespective of their size. Mathematically, it measures the cosine of the angle between two vectors projected in a multi-dimensional space. The cosine similarity is advantageous because even if the two similar documents are far apart by the Euclidean distance (due to the size of the document), chances are they may still be oriented closer together. The smaller the angle, higher the cosine similarity.
<br>
![Screenshot (18)](https://github.com/user-attachments/assets/8877f899-a78d-43a7-8028-d7e35681102c)
<br>
More about Cosine Similarity : [Understanding the Math behind Cosine Similarity](https://www.machinelearningplus.com/nlp/cosine-similarity/)

# Sources of the Datasets:
1. [IMDB 5000 Movie Dataset](https://www.kaggle.com/datasets/carolzhangdc/imdb-5000-movie-dataset)
2. [The Movies Dataset](https://www.kaggle.com/datasets/rounakbanik/the-movies-dataset)
3. [List of movies in 2018](https://en.wikipedia.org/wiki/List_of_American_films_of_2018)
4. [List of movies in 2019](https://en.wikipedia.org/wiki/List_of_American_films_of_2019)
5. [List of movies in 2020](https://en.wikipedia.org/wiki/List_of_American_films_of_2020)

# Final Output
https://github.com/user-attachments/assets/2bfdeeaa-df16-4224-85b8-fb728392bf4c



