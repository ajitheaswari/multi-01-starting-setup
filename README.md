# Multi-Service Starter Setup

A boilerplate project that demonstrates how to build and run a **multi-container Docker setup** using Node.js, Express, React, and MongoDB. Ideal for developers learning Docker concepts like **bind mounts**, **named volumes**, and **service orchestration**.

---

## 📁 Project Structure

multi‑01‑starting‑setup/
├── backend/
│   ├── Dockerfile
│   ├── package.json
│   └── src/
│       └── server.js
├── frontend/
│   ├── Dockerfile
│   ├── package.json
│   └── src/
│       └── App.js
├── docker-compose.yml
└── README.md


- `backend/`: Node.js + Express API
- `frontend/`: React app served in development mode
- `docker-compose.yml`: Defines and runs all services
- `mongo`: Official MongoDB service with data persistence

---

## 🚀 Features

- 🧱 Full-stack Dockerized environment
- ♻️ Hot reloading via bind mounts
- 💾 MongoDB data persistence via named volume
- 🔁 Seamless communication between services over Docker network

---

## 📦 Requirements

- [Docker](https://www.docker.com/products/docker-desktop)
- [Docker Compose](https://docs.docker.com/compose/install/)

---

## 🛠️ Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/ajitheaswari/multi-01-starting-setup.git
   cd multi-01-starting-setup
Run the multi-container app:

bash
Copy
Edit
docker-compose up --build
Access services:

Frontend: http://localhost:3000

Backend: http://localhost:4000

MongoDB: Accessible to backend via service name mongo

🔄 Live Development
Backend files are bind-mounted; any changes in backend/src auto-restart the server.

Frontend React app supports hot reload out of the box.

MongoDB volume ensures data is retained between container restarts.

🧹 Cleanup
To stop and remove containers, networks, and volumes:

bash
Copy
Edit
docker-compose down --volumes
To remove the persistent MongoDB volume:

bash
Copy
Edit
docker volume rm multi-01-starting-setup_mongo-data
⚙️ Customization Ideas
Component	Suggested Enhancements
Backend	Add environment variable support, logging, authentication
Frontend	Add routing, UI frameworks, API integration
Docker	Add environment-specific configs, health checks

📄 License
This project is licensed under the MIT License — free to use and modify.
