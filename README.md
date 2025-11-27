This project is a React.js Movie Explorer application that allows users to browse popular movies, search films, and manage a personalized list of favorite movies.

🔥 Features

Browse Popular Movies: Fetches trending films from TheMovieDB API when the app loads.

Search Functionality: Users can search for movies by title using the TMDB search endpoint.

Add to Favorites: Each movie has a heart button that toggles favorite status.

Persistent Favorites: Favorites are stored using localStorage, so the list remains even after reloading the page.

React Context API: Global movie state (favorites list, add/remove functions, checks) is handled through a custom MovieContext provider.

Reusable UI Components: Includes MovieCard component for all movie listings and a Favorites page to display saved movies.

Responsive Layout: Clean grid layout for both Home and Favorites pages.

🧩 Core Architecture

Home Page:

Fetches popular movies using getPopularMovies().

Handles movie search using searchMovies(query).

Renders results using MovieCard components.

Favorites Page:

Reads favorites from MovieContext.

Displays the user’s saved movies in a grid layout.

MovieContext:

Stores favorites array globally.

Provides functions: addToFavorites, removeFromFavorites, and isFavorite.

Syncs favorites to localStorage.

MovieCard Component:

Displays poster, title, release year.

Heart button toggles favorites.

🛠️ Tech Stack

React.js (Hooks, Context API)

JavaScript (ES6+)

TMDB API

LocalStorage

CSS (Responsive Grid + Overlay Effects)
