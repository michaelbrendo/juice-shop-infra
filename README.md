# Juice Shop Infrastructure

This repository manages the **System Under Test (SUT)** for my automated testing ecosystem. It uses the **OWASP Juice Shop**, a modern web application, containerized for consistent test execution across different environments.

## Architecture
- **Environment**: Linux (WSL 2)
- **Engine**: Docker & Docker Compose
- **Service**: Node.js / Express / Angular (OWASP Juice Shop)

## Getting Started

### Prerequisites
- Docker.
- Git.

### Setup
1. Clone the repository:
2. Spin up the environment: 
```bash
docker compose up -d
```
3. Verify if the application is healthy: 
```bash
docker ps
```
The application will be available at http://localhost:3000.

### Observability & Troubleshooting
To check the server-side logs during test execution (useful for debugging 5xx errors or API crashes):
```bash
- docker compose logs -f juice-shop
```

### License
This project is licensed under the MIT License - see the [LICENSE](./LICENSE) file for details.