[![Open in Codespaces](https://classroom.github.com/assets/launch-codespace-2972f46106e565e64193e422d61a12cf1da4916b45550586e14ef0a7c637dd04.svg)](https://classroom.github.com/open-in-codespaces?assignment_repo_id=22849504)

# CSSE6400 Week 1 Practical — Todo API

A simple REST API for managing todo items, built with Flask and Python.

## Requirements

- Python 3.12+
- [Poetry](https://python-poetry.org/)

## Setup

```bash
poetry install --no-root
```

## Running

```bash
poetry run flask --app todo run -p 6400
```

The API is available at `http://localhost:6400/api/v1`.

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/api/v1/health` | Health check |
| `GET` | `/api/v1/todos` | List all todos |
| `GET` | `/api/v1/todos/<id>` | Get a todo |
| `POST` | `/api/v1/todos` | Create a todo |
| `PUT` | `/api/v1/todos/<id>` | Update a todo |
| `DELETE` | `/api/v1/todos/<id>` | Delete a todo |

## Testing

```bash
poetry run python3 -m unittest discover -s tests
```
