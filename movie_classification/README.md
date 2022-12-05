# Movie classification

This repo contains content from the December 6, 2022 [Kansas City Graph Data Science Meetup](https://www.meetup.com/kansas-city-graph-databases-meetup-group/events/290004971/).

## Setting up the data

The fastest way to get started with the data is to download the Neo4j dump file from this location:
http://nsmith-neo4j-blogs.s3.amazonaws.com/movie-classification/movies.dump. This dump file was prepared in 
November, 2022 and contains information from https://www.themoviedb.org/ for movies released between January 1, 1980
and November of 2022.

Once you have downloaded the dump file, you can [load it to a database in Neo4j Desktop](https://tbgraph.wordpress.com/2020/11/11/dump-and-load-a-database-in-neo4j-desktop/) or 
[load it in an AuraDS instance](https://aura.support.neo4j.com/hc/en-us/articles/1500011497162-Loading-Data-into-Neo4j-Aura#Method2).
If you use a Neo4j Desktop database, make sure you [install the APOC and Graph Data Science plugins](https://neo4j.com/docs/desktop-manual/current/operations/install-plugin/).

If you would prefer to download your own more current dataset, you can sign up for
a free API key from themoviedb.org. Set up a Neo4j database to receive the movie information.
Use your TMDB API key and Neo4j database information to update the first few cells Download_TMDB_movies.ipynb notebook.
Then run the notebook. It takes a while to download a large volume of movies.

## Running the classification notebook
Once you have the database set up, you can run the Classify_movie_profitability.ipynb notebook.
Update the first few cells to point the Neo4j connection to your database.
