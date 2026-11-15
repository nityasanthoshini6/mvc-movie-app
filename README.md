# MVC Movie API

A RESTful backend API built with Node.js, Express, and MongoDB using the **MVC** architecture for managing movie records.

## Tech Stack
* **Runtime:** Node.js (ES Modules)
* **Framework:** Express.js
* **Database:** MongoDB & Mongoose

## Project Structure
```text
movie-api/
├── config/db.js
├── controllers/movieController.js
├── models/movieModel.js
├── routes/movieRoutes.js
├── .env / .gitignore
├── package.json
└── server.js
```

## Setup & Installation

1. **Clone & Install**
   ```bash
   git clone <your-repo-url>
   cd movie-api
   npm install
   ```

2. **Configure `.env`**
   ```env
   PORT=9000
   MONGO_URI=mongodb://127.0.0.1:27017
   DB_NAME=movieDB
   ```

3. **Start the server**
   ```bash
   npm start
   ```
   Runs locally at `http://localhost:9000`.

## API Endpoints

* `GET /` — Health check
* `GET /api/v1/movies` — Get all movies
* `GET /api/v1/movies/:id` — Get movie by ID
* `POST /api/v1/movies` — Create a movie
* `PUT /api/v1/movies/:id` — Update a movie
* `DELETE /api/v1/movies/:id` — Delete a movie

### Example `POST` Body
```json
{
  "title": "Inception",
  "category": "Sci-Fi",
  "year": 2010
}
```
