# Basic Goal Manager (Flask + FastAPI)

This project is a simple goal manager app with:

- Backend option 1: Flask
- Backend option 2: FastAPI
- Frontend: HTML, CSS, JavaScript

Both backends serve the same frontend and expose the same REST API.

## Features

- Add goals
- List goals
- Mark goals done/open
- Delete goals
- Data is stored in `data/goals.json`

## Setup

1. Create and activate a virtual environment (recommended)
2. Install dependencies:

```bash
pip install -r requirements.txt
```

## Run with Flask

```bash
python backend/flask_app/app.py
```

Open: `http://127.0.0.1:5000`

## Run with FastAPI

```bash
uvicorn backend.fastapi_app.main:app --reload --port 8000
```

Open: `http://127.0.0.1:8000`

## API Endpoints

- `GET /api/goals`
- `POST /api/goals`
- `PUT /api/goals/{goal_id}`
- `DELETE /api/goals/{goal_id}`

### Example POST body

```json
{
  "title": "Read 20 pages",
  "description": "Start with chapter 3",
  "target_date": "2026-03-30"
}
```
# goalmanager-workflow-github-actions-
