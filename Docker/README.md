## 🐳 Run Locally with Docker

You can run the entire 3-tier app locally using Docker and Docker Compose.

### ▶️ Prerequisites:
- Docker installed
- Docker Compose installed

### 📁 File Used:
- `docker/docker-compose.yaml`
- `docker/Dockerfile` (if applicable)
- `app/`, `database/`

### 🚀 Steps:

```bash
cd docker
docker-compose up --build
```

This will:

- ✅ Build and run frontend (app/client)

- ✅ Build and run backend (app/backend)

- ✅ Set up MySQL container (database/mysql)

- ✅ Connect all services using Docker networking

- ➡️ Access the frontend at: http://localhost:3000
