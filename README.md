
![Alt text](https://www.google.com/imgres?imgurl=https%3A%2F%2Fwww.oscars.org%2Fsites%2Foscars%2Ffiles%2F91o_news-image_generic.png&imgrefurl=https%3A%2F%2Fwww.oscars.org%2Fnews%2Facademy-determines-new-oscars-category-merits-further-study&docid=KavP9YC0VCkzwM&tbnid=5i11NpYX-Oz84M%3A&vet=10ahUKEwji07LzqZDiAhVGbKwKHbJmD_wQMwh7KC0wLQ..i&w=1433&h=806&client=safari&bih=714&biw=1240&q=Oscar%20png%20images&ved=0ahUKEwji07LzqZDiAhVGbKwKHbJmD_wQMwh7KC0wLQ&iact=mrc&uact=8)
# ETL-project
Authors: Leeza Sergeeva, Alina Smirnova, Anna Burlyaeva

## Idea
To create a pipeline to analyze the popularity of movies made in San Francisco. A movie’s popularity rate can be measured as a count of awards.

## Data sources

1. https://data.sfgov.org/Culture-and-Recreation/Film-Locations-in-San-Francisco/yitu-d5am
2. https://www.kaggle.com/theacademy/academy-awards
3. https://www.kaggle.com/carolzhangdc/imdb-5000-movie-dataset
4. https://www.kaggle.com/rounakbanik/the-movies-dataset#movies_metadata.csv

Possible types of transformation: 
* cleaning
* joining
* filtering
* aggregating

Final database can include: movie_name, year, actors, awards, gross_income, budget, etc.

## Results

### Final pipeline includes three steps:

1.	Extraction: extracted three datasets – movies names and other attributes made in San Francisco, awards data, budget and gross income data;
2.	Transformation: three datasets were combined and filtered by location, a count of awards by movie and a count of awards by movie and actor were calculated, three dataframes (actors, movies_awards, movies_actors_awards) were created;
3.	Loading: created dataframes were loaded into SQLite Database
