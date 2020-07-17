Movie API

An API interface to search and find movies by names, directors and genres.

It uses data from imdb.json

## Setting up project and initializing data
```
# create a virtualenv 
virtualenv myvenv
source myvenv/bin/activate
pip install -r reuqirements.txt
./manage.py migrate
./manage.py runserver 7001
./manage.py populate_movies
```


API request examples

base API url
http://127.0.0.1:7001/api/movies

filter by name (full text search)
http://127.0.0.1:7001/api/movies?name=wizard

filter by movie name and director name
http://127.0.0.1:7001/api/movies?name=wizard&director=victor

filter by genre name
http://127.0.0.1:7001/api/movies?genre=family
