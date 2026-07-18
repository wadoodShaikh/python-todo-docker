# Python To-Do App (Docker Compose)

A simple Flask-based To-Do web application, containerized with Docker and orchestrated with Docker Compose.

## Features

- Add a new task
- View all tasks
- Delete a task
- Mark a task as completed (toggle)

## Project Structure

```
python-todo-app/
│
├── app.py
├── requirements.txt
├── Dockerfile
├── docker-compose.yml
├── .gitignore
├── templates/
│   └── index.html
└── static/
    └── style.css
```

## Run Locally (without Docker)

```bash
pip install -r requirements.txt
python app.py
```

Visit http://localhost:5000

## Run with Docker Compose

```bash
docker compose up --build
```

Visit http://localhost:5000

To stop:

```bash
docker compose down
```

## Upload to GitHub

```bash
git init
git add .
git commit -m "Initial commit - Python Todo App with Docker Compose"
git remote add origin https://github.com/<your-username>/python-todo-docker.git
git branch -M main
git push -u origin main
```

## Tech Stack

- Python 3.10
- Flask
- SQLite (file-based, no separate DB container needed)
- Docker & Docker Compose
