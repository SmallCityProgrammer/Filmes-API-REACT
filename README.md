# Movies Library App

This application displays information about movies using The Movie Database (TMDb) API.

## Components

### Home Component
#### Location: src/pages/Home.js

The Home component fetches the top-rated movies from the API and displays them on the home page. It uses the `useState` and `useEffect` hooks from React to manage state and perform side effects (like fetching data). The `getTopRatedMovies` function fetches the top-rated movies from the API using an async/await approach. Once the data is fetched, it updates the state using `setTopMovies` which triggers a re-render to display the fetched movies.

### Search Component
#### Location: src/pages/Search.js

The Search component is responsible for displaying search results based on a query parameter received through the URL. It uses the `useSearchParams` hook from `react-router-dom` to get the search query from the URL. The `getSearchedMovies` function fetches the movies based on the search query from the API and updates the state to display the search results.

### MovieCard Component
#### Location: src/components/MovieCard.js

The MovieCard component is a reusable component used to display information about a single movie. It takes the `movie` object as a prop and displays the movie poster, title, and average rating. Additionally, it provides a link (if `showLink` is true) to the details of the movie.

### Navbar Component
#### Location: src/components/Navbar.js

The Navbar component provides navigation and search functionality. It contains a navigation link to the home page and a search bar. When users type a query in the search bar and submit it, they're redirected to the search page (`/search?q=<query>`), allowing them to see search results based on the query.

## Technologies Used

- React
- React Router
- Fetch API

## Setup Instructions

1. Clone the repository.
2. Install dependencies: `npm install`
3. Start the development server: `npm start`
4. Access the application in your browser at `http://localhost:3000/`

## Credits

This application was made in accordance with the videos from Matheus Battisti
