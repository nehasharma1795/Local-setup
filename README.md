# 📝 Todo Application

A full-stack Todo application built with **FastAPI** (backend) and **React.js** (frontend), containerized with Docker and deployed via a **CI/CD pipeline using GitHub Actions**.

---

## 📦 Tech Stack

- **Frontend**: React.js
- **Backend**: FastAPI (Python 3.10)
- **Containerization**: Docker
- **CI/CD**: GitHub Actions
- **Database**: SQLite (local)
- **Deployment**: Docker Compose

---

## 🗂️ Project Structure

```
todo-application/
├── backend/               # FastAPI backend
│   └── Dockerfile
├── frontend/              # React app
│   └── todo/
│       └── Dockerfile
├── docker-compose.yml     # Service composition
└── .github/workflows/
    └── deploy.yml         # GitHub Actions workflow
```

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
cd /automating-CICD/todo-application/
git clone https://github.com/nehasharma1795/todo-app-deployment.git 
cd todo-application
```

### 2. Build and Run with Docker Compose

```bash
docker-compose up --build
```

- Backend: [http://localhost:8000/docs](http://localhost:8000/docs)
- Frontend: [http://localhost:3000](http://localhost:3000)

---

## 🔁 CI/CD with GitHub Actions

### Trigger

- Every `push` or `merge` to the `main` branch

### Actions

1. Build Docker images for backend and frontend
2. Push to Docker Hub 

### Secrets Required

- `DOCKER_USERNAME`
- `DOCKER_PASSWORD`

> Add these under **Repo Settings → Secrets and variables → Actions**

---

## 🐳 Docker Image Info

- **Backend Image**: `your-username/todo-backend:latest`
- **Frontend Image**: `your-username/todo-frontend:latest`

---

## 🔧 API Endpoints (FastAPI)

| Method | Endpoint         | Description      |
|--------|------------------|------------------|
| GET    | `/tasks`         | List all tasks   |
| POST   | `/tasks`         | Create a new task|
| PUT    | `/tasks/{id}`    | Update a task    |
| DELETE | `/tasks/{id}`    | Delete a task    |

Visit Swagger docs at: [http://localhost:8000/docs](http://localhost:8000/docs)

---

## 💡 Future Enhancements

- Add authentication
- Persist data in PostgreSQL
- Deploy to Kubernetes using Helm and ArgoCD

---

##  Author NEHA SHARMA

**Your Name**  
LinkedIn: [neha sharma](https://www.linkedin.com/in/neha-sharma1795/)  
GitHub: [@nehasharma1795](https://github.com/nehasharma1795)

