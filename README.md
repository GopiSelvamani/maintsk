Here’s a basic structure and content for a README file for your GitHub repository that you can use to submit your work. This file should be placed at the root of your repository.

---

# Movie Search Application

This project is a full-featured movie search application built using React. It integrates with the OMDB API to allow users to search for movies, view detailed information, and manage a list of favorites. The application is responsive and styled using Tailwind CSS.

## Features

- **Search Functionality**: Allows users to search for movies by title or keyword.
- **Movie Details**: Displays detailed information about the movie, including a larger poster, release year, genre, plot summary, ratings, and cast.
- **Pagination**: Handles large sets of search results with pagination to navigate through multiple pages of results.
- **Filter by Type**: Filters search results based on movie type (e.g., movie, series, episode).
- **Favorites**: Users can manage their favorite movies.
- **Error Handling**: Displays appropriate error messages for API request failures or if no results are found.

## Tech Stack

- **React**: For building the user interface.
- **React Router**: For navigation between different pages of the application.
- **OMDB API**: For fetching movie data.
- **Tailwind CSS**: For styling and responsive design.
- **JavaScript**: For implementing functionality like search, filtering, and error handling.

## Setup

To run this project locally, follow the steps below:

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/movie-search-app.git
   ```

2. Navigate into the project folder:

   ```bash
   cd movie-search-app
   ```

3. Install the necessary dependencies:

   ```bash
   npm install
   ```

4. Create a `.env` file at the root of the project and add your OMDB API key:

   ```env
   REACT_APP_OMDB_API_KEY=your_api_key_here
   ```

   You can get an API key by signing up on the [OMDB API website](https://www.omdbapi.com/apikey.aspx).

5. Start the development server:

   ```bash
   npm start
   ```

6. Open your browser and go to `http://localhost:3000` to view the application.

## Deployment

The application is deployed on Netlify. You can view it live here:

[Movie Search Application](https://your-app-name.netlify.app)

## Usage

- On the home page, enter a movie title or keyword in the search bar to see the results.
- Use the dropdown to filter the search results based on movie type (e.g., movie, series).
- Click on a movie to view detailed information including the plot, ratings, cast, and more.
- Add movies to your favorites list.

## Error Handling

- If there is an issue with the API request (e.g., no internet connection), an error message will be displayed.
- If no results are found, a "No movies found" message will be shown.

## Folder Structure

```
/public
  /index.html
/src
  /components
    SearchBar.js
    MovieCard.js
    MovieDetail.js
    Pagination.js
    FilterDropdown.js
  /contexts
    FavoriteContext.js
  /services
    apiService.js
  App.js
  index.js
  tailwind.config.js
  .env
  README.md
```
## Screen Shot of Movie Search

<img width="1431" alt="Screenshot 2025-02-13 at 10 51 25 AM" src="https://github.com/user-attachments/assets/e174cf4c-c375-4171-8b5d-6bac57bf6eba" />

<img width="1429" alt="Screenshot 2025-02-13 at 10 53 13 AM" src="https://github.com/user-attachments/assets/b9095b11-202a-44a8-a8d9-57b9142aab93" />




## Development Notes

- The application uses **React Router** to handle navigation between the search page and the movie details page.
- The **OMDB API** is used for fetching movie data. The API service functions are located in the `/services/apiService.js` file.
- The filter for movie type is implemented by sending a parameter to the API request without using the JavaScript `.filter()` method on arrays.
- The application is styled with **Tailwind CSS** for a responsive and clean design.

## License

This project is open-source and available under the MIT License.

---

Feel free to modify this README as needed based on the specific details of your project. Make sure to replace placeholders like `your-username` and `your-api-key-here` with your actual GitHub username and OMDB API key.

