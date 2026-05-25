# Learn Microservices - Security Module

This repository contains a modular introduction to security in microservice architectures using OAuth2, JWTs, Keycloak, Spring Security and NGINX.

The project combines theoretical concepts with practical demonstrations in order to illustrate how authentication and authorization can be implemented inside distributed systems.

---

## Repository Structure

```text
modules/
code/
```

- `modules/` contains the theoretical chapters and practical demonstrations.
- `code/` contains the Docker, Keycloak, NGINX and Spring Boot configurations used throughout the module.

---

## Chapters

### Chapter I — OAuth2 Foundations
Introduction to:
- OAuth2;
- access tokens;
- refresh tokens;
- Authorization Code Flow;
- Service Account Flow.

### Chapter II — Keycloak Demo
Practical demonstration of:
- Keycloak configuration;
- realm creation;
- client configuration;
- user authentication;
- token retrieval through OAuth2 flows.

### Chapter III — Protecting Microservices with JWT Validation
Introduction to:
- JWT validation in distributed systems;
- Spring Security OAuth2 Resource Server;
- decentralized authentication;
- token propagation between microservices.

### Chapter IV — Centralizing Authorization with NGINX Gateway
Introduction to:
- API Gateway architectures;
- centralized authorization;
- NGINX routing;
- NJS-based authorization logic.

### Chapter V — NGINX Gateway Demo
Practical demonstration of:
- gateway-based request filtering;
- JWT validation;
- authorization enforcement;
- authenticated and unauthorized request handling.

---

## Technologies Used

- Docker
- Spring Boot
- Spring Security
- Keycloak
- OAuth2
- JWT
- NGINX
- NJS

---

## Running the Environment

From the `code/` directory:

```bash
docker compose up --build
```

Before starting the environment, the microservices must first be compiled through Gradle in order to generate the required `.jar` artifacts.

---

## Final Notes

This module demonstrates a layered security architecture for modern distributed systems in which:
- authentication is delegated to an Identity Provider;
- JWT validation is distributed across services;
- authorization policies can be centralized through an API Gateway.

The final architecture combines scalability, modularity and separation of concerns while maintaining secure communication between microservices.