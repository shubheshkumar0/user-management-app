# 🚀 User Management System

A full-stack user management application demonstrating Docker containerization concepts.

![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)

## 🛠️ Tech Stack

- **Frontend**: HTML, CSS, JavaScript (Nginx)
- **Backend**: Node.js, Express.js
- **Database**: MongoDB
- **Containerization**: Docker & Docker Compose

## 📦 Docker Concepts Demonstrated

- ✅ Multi-container orchestration with Docker Compose
- ✅ Custom Dockerfiles for frontend and backend
- ✅ Docker volumes for data persistence
- ✅ Container networking
- ✅ Port mapping and exposure
- ✅ Environment variables configuration

## 🚀 Quick Start

### Prerequisites
- Docker Desktop installed ([Download here](https://www.docker.com/products/docker-desktop))
- Git

### Installation & Setup

1. **Clone the repository**:
```bash
git clone https://github.com/shubheshkumar0/user-management-app.git
cd user-management-app
```

2. **Start the application**:
```bash
docker-compose up --build
```

3. **Access the application**:
   - Frontend: http://localhost:8080
   - Backend API: http://localhost:3000/api/users
   - MongoDB: localhost:27017

## 🎯 Features

- ✅ Add users with name, email, and role
- ✅ View all users with real-time statistics
- ✅ Delete users with confirmation
- ✅ Data persistence using Docker volumes
- ✅ Modern, responsive UI with animations
- ✅ Role-based user management (Admin, Manager, User)

## 📁 Project Structure
```
user-management-app/
├── docker-compose.yml          # Multi-container orchestration
├── frontend/
│   ├── Dockerfile             # Nginx container config
│   ├── index.html             # Frontend UI
│   └── nginx.conf             # Nginx server config
└── backend/
    ├── Dockerfile             # Node.js container config
    ├── package.json           # Node dependencies
    ├── server.js              # Express API server
    └── .dockerignore          # Docker ignore file
```

## 🐳 Docker Architecture
```
┌─────────────────────────────────────────────────────┐
│                  Docker Compose                      │
├─────────────────┬─────────────────┬─────────────────┤
│   Frontend      │    Backend      │    MongoDB      │
│   (Nginx)       │   (Node.js)     │   (Database)    │
│   Port: 8080    │   Port: 3000    │   Port: 27017   │
└─────────────────┴─────────────────┴─────────────────┘
         │                 │                 │
         └─────────────────┴─────────────────┘
                  app_network (Bridge)
```

## 🔧 Useful Docker Commands
```bash
# Start containers in detached mode
docker-compose up -d

# View running containers
docker ps

# View logs
docker-compose logs -f

# Stop containers
docker-compose down

# Remove containers and volumes (deletes data)
docker-compose down -v

# Rebuild containers
docker-compose up --build
```

## 📊 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/api/users` | Get all users |
| POST | `/api/users` | Create a new user |
| DELETE | `/api/users/:id` | Delete a user |

## 🎓 Learning Outcomes

This project demonstrates:
- Docker containerization
- Multi-container application deployment
- Docker Compose orchestration
- Volume management for data persistence
- Container networking
- Building production-ready Docker images
- REST API development with Node.js
- Frontend-Backend-Database integration

## 📚 Resources

Built following [TechWorld with Nana's Docker Tutorial](https://www.youtube.com/c/TechWorldwithNana)

## 👨‍💻 Author

**Shubhesh Kumar**
- GitHub: [@shubheshkumar0](https://github.com/shubheshkumar0)

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

---

⭐ If you found this project helpful, please give it a star!