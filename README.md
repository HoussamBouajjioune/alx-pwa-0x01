# ALX Project 0x14 - CineSeek API Integration

This project involves integrating the MoviesDatabase API into a modern movie discovery app built with Next.js, TypeScript, and Tailwind CSS. The goal is to demonstrate understanding of API documentation and build a scalable, responsive frontend that consumes movie data effectively.

---

## API Overview

The MoviesDatabase API provides programmatic access to a rich dataset of movies, series, genres, actors, and related information. Key features include:

- Search for movies by title, genre, or release year.
- Retrieve detailed information about a specific movie or TV show.
- Support for filtering and sorting results.
- Pagination to manage large datasets.
- Access to images, descriptions, ratings, and more.

---

## Version

**API Version:** v1

---

## Available Endpoints

| Endpoint                     | Description |
|-----------------------------|-------------|
| `/titles`                   | Retrieves a list of movies or TV shows. Supports filters like year, genre, etc. |
| `/titles/:id`               | Fetches detailed info for a specific title by ID. |
| `/genres`                   | Returns a list of all available genres. |
| `/actors/:id`               | Returns details about a specific actor. |
| `/titles/search/title`      | Search for movies or series by title name. |

---

## Request and Response Format

### Sample Request

```http
GET /titles?year=2022&genre=Action&page=1
Host: moviesdatabase.p.rapidapi.com
Headers:
  X-RapidAPI-Key: your_api_key
  X-RapidAPI-Host: moviesdatabase.p.rapidapi.com
