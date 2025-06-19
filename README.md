# ALX Movie App

## API Overview

The Movie Database API is a powerful web service providing developers with programmatic access to a vast and continuously updated collection of data about movies, TV shows, and entertainment industry professionals. It's an invaluable resource for building applications that require rich content information, from discovery tools to personalized recommendation systems.

### Key Features:

* **Comprehensive Data:** Offers extensive details for movies, TV shows (including seasons and episodes), and people (actors, directors, crew), encompassing titles, synopses, genres, ratings, cast/crew credits, budgets, and more.
* **Rich Media:** Provides access to high-resolution images (posters, backdrops) and video links (trailers), enhancing the visual appeal of applications.
* **Powerful Search & Discovery:** Includes robust search functionalities for content and people, alongside "discover" endpoints for filtering and retrieving content based on various criteria like popularity, genre, release year, and streaming availability.
* **User Interaction (Auth Required):** Supports user-centric features such as creating watchlists, rating content, and managing custom lists, typically requiring API key authentication and user session management.
* **Localization Support:** Offers configuration data for image paths and lists of languages/countries, aiding in building localized applications.

## API Version

As of the current documentation, the primary version of the TMDb API is **v3**.

## Available Endpoints

Here are some of the main endpoint categories available:

* **`/movie`**: Access details about individual movies, including popular, top-rated, upcoming, and specific movie details.
    * Example: `/movie/{movie_id}`
* **`/tv`**: Retrieve information about TV shows, including popular, top-rated, and specific TV show details, seasons, and episodes.
    * Example: `/tv/{tv_id}/season/{season_number}/episode/{episode_number}`
* **`/person`**: Get details about individual people (actors, directors), including their filmography.
    * Example: `/person/{person_id}`
* **`/search`**: Search for movies, TV shows, and people by keyword.
    * Example: `/search/movie`
* **`/discover`**: Powerful endpoints to discover movies or TV shows based on various criteria (e.g., genre, release date ranges, vote counts).
    * Example: `/discover/movie`
* **`/configuration`**: Provides static data necessary for using the API, such as image base URLs and valid language codes.
    * Example: `/configuration`

## Request and Response Format

The TMDb API primarily uses **JSON** for both request bodies (where applicable, like for adding items to lists) and all responses.

### Typical Request Structure (GET):

Most requests are GET requests with parameters passed as query strings.
