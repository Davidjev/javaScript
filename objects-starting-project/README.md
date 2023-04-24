# Movie Database App

This is a simple movie database application built with JavaScript. Users can add new movies to the database and search for movies by title.

### Functionality

The application provides the following functionality:

- Add new movies to the database  
- Search for movies by title

### Usage

To use the application, simply clone the repository and open index.html in your web browser.

### Code

The main code for the application is contained in the script.js file. It defines the following variables and functions:

#### Variables

- addMovieBtn: Gets the "Add Movie" button from the HTML document.  
- searchBtn: Gets the "Search" button from the HTML document.  
- movies: An array that stores all the movies in the database.

#### Functions

- renderMovies(filter = ''): Renders the list of movies in the HTML document. It takes an optional filter parameter that allows the user to filter the movies by title.  
- addMovieHandler(): Adds a new movie to the database when the "Add Movie" button is clicked.  
- searchMovieHandler(): Searches for movies by title when the "Search" button is clicked.

