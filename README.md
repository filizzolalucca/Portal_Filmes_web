# Portal dos Filmes

A movie portal website built with plain HTML, CSS and JavaScript. It pulls live data from [The Movie Database (TMDB) API](https://developer.themoviedb.org/) to show what's in theaters, browse movies by genre, search, and open a details page for each title.

<p>
  <img src="https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white" alt="HTML5">
  <img src="https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white" alt="CSS3">
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black" alt="JavaScript">
  <img src="https://img.shields.io/badge/Bootstrap-7952B3?logo=bootstrap&logoColor=white" alt="Bootstrap">
</p>

> The site's content is in Brazilian Portuguese.

## Pages

| Page | What it does |
|---|---|
| `index.html` | Home: movies now playing, highlights filtered by genre, latest reviews, interviews and news sections |
| `pesquisa.html` | Search for movies and TV shows, with paginated results |
| `filme.html` | Movie details: poster, synopsis, genres, rating, runtime, release date, budget, production companies and official website |

## How it works

- Requests are made with `XMLHttpRequest` to TMDB endpoints such as `movie/now_playing`, `discover/movie`, `genre/movie/list`, `search/multi` and `movie/{id}`
- Results are rendered into the page with template strings
- The search query, page number and movie id are passed between pages through URL parameters
- Layout and components come from Bootstrap, with jQuery and Font Awesome

## Getting started

1. Clone the repository:
   ```bash
   git clone https://github.com/filizzolalucca/Portal_Filmes_web.git
   ```
2. Get a free API key at [themoviedb.org](https://www.themoviedb.org/settings/api) and set it in the `API_KEY` constant at the top of `index.js`, `filme.js` and `pesquisa.js`.
3. Open `index.html` in your browser.

## Author

**Lucca Filizzola** · [@filizzolalucca](https://github.com/filizzolalucca)
