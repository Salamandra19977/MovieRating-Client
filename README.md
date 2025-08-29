API-> https://api.themoviedb.org/3/movie/popular?api_key=${TMDB_API_KEY}&language=en-US&page=1
DB-> https://supabase.com/
Backend-> https://movierating-server.onrender.com/

Frontend-> https://salamandra19977.github.io/MovieRating-Client
Server status-> GET:https://movierating-server.onrender.com/api/health
Sync with API-> POST:https://movierating-server.onrender.com/api/movies/sync

Test user:
username: Robocode
password: Robocode

Server
|   .env
|   package-lock.json
|   package.json
|   server.js
|
+---controllers
|       authController.js
|       commentsController.js
|       moviesController.js
|
+---db
|       index.js
|
+---logs
|       app.log
|
+---middleware
|       authMiddleware.js
|       logger.js
+---migrations
|       shema.sql
+---routes
|       auth.js
|       comments.js
|       movies.js
|
\---services
        externalMovieService.js

Client
|   .env
|   index.html
|   package-lock.json
|   package.json
|   vite.config.js
|
+---dist
|   |   index.html
|   |
|   \---assets
|           index-iRVE4RJl.js
|           index-xBbIuU8m.css
|
\---src
    |   App.jsx
    |   index.jsx
    |
    +---api
    |       api.js
    |
    +---components
    |       CommentForm.jsx
    |       CommentList.jsx
    |       MovieCard.jsx
    |       MovieList.jsx
    |       ReactionButtons.jsx
    |
    +---contexts
    |       AuthContext.jsx
    |
    +---pages
    |       Home.jsx
    |       Login.jsx
    |       MoviePage.jsx
    |       Register.jsx
    |
    +---styles
    |       main.scss
    |       _variables.scss
    |
    \---utils
            time.js