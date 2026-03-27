# 🧪 Testing Sandbox 2024 — ELTE University

> A software testing sandbox environment built at **ELTE University**, featuring a Dockerized setup with automated test suites covering HTML, JavaScript, Java, and CSS components.

---

## 📋 Table of Contents

- [About](#about)
- [Project Structure](#project-structure)
- [Tech Stack](#tech-stack)
- [Getting Started](#getting-started)
- [Running Tests](#running-tests)
- [Docker Setup](#docker-setup)

---

## About

This repository is a **software testing sandbox** developed as part of the Software Testing course at ELTE University's Computer Science program. It provides a containerized environment for writing and running automated tests across a multi-language web application.

---

## Project Structure

```
elte/
├── tests/                        # Test suites
├── Dockerfile                    # Docker image definition
├── docker-compose.yml            # Multi-container orchestration
├── testing-sandbox-2024.zip      # Project archive
└── README.md
```

---

## Tech Stack

| Layer | Technology |
|-------|-----------|
| **Frontend** | HTML, CSS, JavaScript |
| **Backend** | Java |
| **Containerization** | Docker, Docker Compose |
| **Testing** | Automated test suites (see `/tests`) |

---

## Getting Started

### Prerequisites

- [Docker](https://www.docker.com/) installed
- [Docker Compose](https://docs.docker.com/compose/) installed

### Clone the Repository

```bash
git clone https://github.com/bahh99/elte.git
cd elte
```

### Start with Docker Compose

```bash
docker-compose up --build
```

This will build the image and spin up all required containers.

To stop:

```bash
docker-compose down
```

---

## Running Tests

Once the containers are running, execute the test suite:

```bash
# Run all tests inside the container
docker exec -it <container_name> ./run-tests.sh
```

Or navigate to the `tests/` directory and run tests directly depending on the test framework used.

---

## Docker Setup

The project uses a `Dockerfile` and `docker-compose.yml` for a fully reproducible environment.

```bash
# Build image manually
docker build -t elte-sandbox .

# Run container
docker run -p 8080:8080 elte-sandbox
```

---

## 📍 University

**ELTE University** — Eötvös Loránd University, Budapest, Hungary
Faculty of Informatics — Computer Science Program

---

<p align="center">
  <img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white"/>
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black"/>
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white"/>
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white"/>
  <img src="https://img.shields.io/badge/ELTE_University-003087?style=for-the-badge"/>
</p>
