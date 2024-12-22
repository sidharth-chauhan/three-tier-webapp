# 3-Tier Web Application

This is a Docker-based 3-tier web application consisting of a React frontend, Flask backend API, and PostgreSQL database.

## Architecture

- Frontend: React application (port 3000)
- Backend: Flask REST API (port 5000)
- Database: PostgreSQL (port 5432)

## Prerequisites

- Docker
- Docker Compose

## Getting Started

1. Clone the repository:
```bash
git clone <repository-url>
cd <repository-name>
```

2. Start the application:
```bash
docker-compose up --build
```

3. Access the application:
- Frontend: http://localhost:3000
- Backend API: http://localhost:5000

## API Endpoints

- GET /api/users - Retrieve all users
- POST /api/users - Create a new user

## Environment Variables

### Backend
- DATABASE_URL: PostgreSQL connection string

### Frontend
- REACT_APP_API_URL: Backend API URL

### Database
- POSTGRES_USER: Database user
- POSTGRES_PASSWORD: Database password
- POSTGRES_DB: Database name

## Development

To make changes to the application:

1. Frontend changes:
   - Modify files in the `frontend/src` directory

2. Backend changes:
   - Modify files in the `backend` directory

3. Rebuild containers after changes:
```bash
docker-compose down
docker-compose up --build
```

## License

MIT
