<div align='center'>

# Sirius Admin

</div>

**Sirius Admin** is a cloud-ready backend administration service built with **FastAPI** and **PostgreSQL**, designed to demonstrate production-level backend architecture and modern DevOps practices.

The service focuses on **high-performance APIs, raw SQL database interactions, and scalable backend design** without relying on ORMs. Authentication is intentionally excluded to allow integration with a dedicated authentication service in a microservice architecture.

---

# 🚀 Features

* ⚡ High-performance APIs built with FastAPI
* 🗄️ Raw SQL queries (no ORM abstraction)
* 🔄 Async database access using connection pooling
* 🧩 Modular backend architecture
* 📊 Admin data management APIs
* 🐳 Containerization-ready structure
* ☁️ Cloud deployment ready
* 🔄 CI/CD friendly repository structure

---

# 🧱 Tech Stack

### Backend

* **FastAPI** – High-performance Python API framework
* **Uvicorn** – ASGI server
* **asyncpg** – Async PostgreSQL driver
* **Pydantic** – Data validation and configuration

### Database

* **PostgreSQL** – Relational database

### DevOps & Tooling

* **Docker** – Containerization
* **GitHub Actions** – CI/CD pipelines
* **Pytest** – Testing framework
* **Black** – Code formatting
* **Flake8** – Linting

---

# 🧩 Architecture Overview

Sirius Admin is designed to operate as a **data administration microservice**. Authentication and authorization can be handled by a separate service or API gateway.

Example architecture:

```
Auth Service
     │
     ▼
API Gateway
     │
     ▼
Sirius Admin
     │
     ▼
PostgreSQL
```

This design reflects **real-world microservice architecture patterns**.

---

# ⚙️ Installation

## 1️⃣ Clone Repository

```bash
git clone https://github.com/your-username/sirius-admin.git
cd sirius-admin
```

## 2️⃣ Create Virtual Environment

```
python -m venv venv
```

Activate environment:

Linux / macOS

```
source venv/bin/activate
```

Windows

```
venv\Scripts\activate
```

## 3️⃣ Install Dependencies

```
pip install -r requirements.txt
```

---

# 🗄️ Database Setup

Install and run **PostgreSQL** locally.

Create database:

```sql
CREATE DATABASE sirius_admin;
```

Configure the database connection using environment variables.

Example:

```
DATABASE_URL=postgresql://postgres:postgres@localhost:5432/sirius_admin
```

---

# ▶️ Running the Application

Start the API server using **Uvicorn**:

```
uvicorn app.main:app --reload
```

API documentation will be available at:

```
http://127.0.0.1:8000/docs
```

---

# 📜 Example API Endpoints

### Users

```
GET /users
GET /users/{id}
POST /users
DELETE /users/{id}
```

### Admin

```
GET /admin/stats
GET /admin/audit-logs
```

---

# 🧪 Running Tests

Run the test suite:

```
pytest
```

---

# 🐳 Docker (Planned)

The project is structured to support containerized deployment using **Docker**.

Example services:

* FastAPI application container
* PostgreSQL database container

---

# ☁️ Cloud Deployment (Planned)

The service can be deployed on modern cloud platforms such as:

* **Amazon Web Services**
* **Google Cloud**
* **Microsoft Azure**

Typical deployment architecture:

```
Internet
   │
Load Balancer
   │
FastAPI Containers
   │
PostgreSQL Database
```

---

# 🎯 Project Goals

Sirius Admin is designed as a **backend engineering and DevOps portfolio project** demonstrating:

* Raw SQL database interactions
* High-performance API development
* Scalable backend architecture
* Microservice-friendly service design
* Cloud-ready infrastructure

---

# 📄 License

This project is released under the MIT License.

---

# 👨‍💻 Author

Developed as a **backend engineering and cloud-focused portfolio project**.

---

If you want, I can now **enhance this README with badges, diagrams, and API examples** so it looks **top-tier on GitHub** and immediately impresses recruiters.

Do you want me to do that next?
