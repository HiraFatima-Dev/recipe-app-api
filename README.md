# Recipe App API

A production-style REST API for managing recipes, built with Django REST 
Framework. Built to practice TDD, Docker-based dev environments, and 
CI/CD with GitHub Actions.

## Features
- User authentication (token-based)
- CRUD for recipes, tags, and ingredients
- Image upload for recipes
- Fully Dockerized dev/prod environments
- Automated testing + linting via GitHub Actions on every push

## Tech Stack
Django · Django REST Framework · PostgreSQL · Docker · GitHub Actions

## Running locally
\`\`\`bash
docker-compose up
\`\`\`
API available at `http://localhost:8000/api/docs`

## Testing
\`\`\`bash
docker-compose run --rm app sh -c "python manage.py test"
\`\`\`

## What I'd improve next
- Add rate limiting
- Swap SQLite → Postgres in prod config
- Add caching layer with Redis
