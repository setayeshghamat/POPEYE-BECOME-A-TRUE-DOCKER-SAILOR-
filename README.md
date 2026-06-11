# Popeye

Docker-based microservices project built with Docker Compose.

The project demonstrates how to design, containerize, and orchestrate a multi-service application using isolated services and reproducible infrastructure.

## Overview

Popeye is a DevOps-oriented project developed at Epitech.

The goal is to build a complete containerized architecture where each service runs in its own Docker container and communicates through a shared Docker Compose environment.

## Architecture

The application is composed of several independent services:

| Service    | Role                                 |
| ---------- | ------------------------------------ |
| Flask      | Backend API                          |
| Redis      | In-memory data store and cache       |
| Java       | Service-oriented application logic   |
| PostgreSQL | Relational database                  |
| Node.js    | Frontend or additional service layer |

The services are orchestrated with Docker Compose.

```text
Flask / Java / Node.js
        ↓
      Redis
        ↓
   PostgreSQL
```

## Features

* Microservices architecture
* Docker containerization
* Multi-container orchestration
* Service-to-service communication
* Environment isolation
* Reproducible local deployment
* Infrastructure automation
* DevOps-oriented workflow

## Tech Stack

* Docker
* Docker Compose
* Flask
* Redis
* Java
* PostgreSQL
* Node.js

## Requirements

* Docker
* Docker Compose

Check Docker installation:

```bash
docker --version
docker compose version
```

## Run

Start all services:

```bash
docker compose up --build
```

Run in detached mode:

```bash
docker compose up --build -d
```

Stop the services:

```bash
docker compose down
```

Stop and remove volumes:

```bash
docker compose down -v
```

## Project Structure

```text
.
├── flask/
├── java/
├── node/
├── postgres/
├── redis/
├── docker-compose.yml
└── README.md
```

## Learning Outcomes

This project focuses on practical DevOps skills:

* Designing container-based systems
* Managing multi-service applications
* Connecting services through Docker networks
* Using Docker Compose for orchestration
* Building portable development environments
* Applying infrastructure and automation principles

## Academic Context

Project: Popeye
School: Epitech – European Institute of Technology
Field: DevOps, Docker, Microservices

## Author

Setayesh Ghamat
