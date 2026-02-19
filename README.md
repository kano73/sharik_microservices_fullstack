**Description:** The shop application is supported by a microservice architecture on the backend (Spring Boot). It uses PostgreSQL, MongoDB, and Redis for data storage, Kafka for microservice communication, and the frontend is implemented with React

---

#  Sharik — Full Stack Microservices Shop

A full stack shop application built with independent microservices. Each service has its own database and communicates via Kafka. Frontend is React, backend is Spring Boot.

---

##  Architecture

* Microservices based backend (Spring Boot)
* Separate databases per service:

  * PostgreSQL
  * MongoDB
  * Redis
* Kafka for event‑driven communication
* React frontend
  This design enables scalability, isolation, and clear service boundaries.

---

##  Tech Stack

**Backend:** Spring Boot
**Frontend:** React
**Databases:** PostgreSQL, MongoDB, Redis
**Messaging:** Kafka
**Containerization:** Docker & Docker Compose

---

##  How to Run

Clone and start with Docker:

```bash
git clone https://github.com/kano73/sharik_microservices_fullstack
# pull latest versions of submodules 
cd sharik_microservices_fullstack
docker compose up --build
```

---

##  Structure

```
services/            # individual microservices
gateway/             # API gateway
frontend/            # React frontend
docker‑compose.yml   # orchestration
```

---

## Development Notes

* Each microservice has its own datastore
* Kafka brokers handle cross‑service events
* React app talks to services via the gateway
