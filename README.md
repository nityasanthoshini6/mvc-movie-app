# MVC Movie API

A RESTful backend API built with Node.js, Express, and MongoDB using the **MVC** architecture for managing movie records.

## Live Deployment (Render)
* **Live API Base URL:** [https://mvc-movie-app-hra4.onrender.com](https://mvc-movie-app-hra4.onrender.com)
* **Movies Endpoint:** [https://onrender.com](https://onrender.com)
*(Note: The Render free-tier server may take 30–50 seconds to wake up on the first request after inactivity.)*

## Tech Stack
* **Runtime:** Node.js (ES Modules)
* **Framework:** Express.js
* **Database:** MongoDB Atlas & Mongoose
* **Hosting:** Render

## Project Structure
```text
mvc-express-app/
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
   git clone https://github.com
   cd mvc-express-app
   npm install
   ```

2. **Configure `.env`**
   ```env
   PORT=9000
   MONGO_URI=your_mongodb_connection_string
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
