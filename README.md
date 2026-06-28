# n8n Birthday Bot Docker

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

A simple Docker setup wrapper configuration for running an instance of [n8n](https://n8n.io/), an extendable workflow automation tool. This setup is prepared for deploying background triggers, specifically designed to coordinate scheduled notifications (like birthday greetings).

---

## 🛠️ Configuration Details

- **Base Image:** `n8nio/n8n:latest`
- **Exposed Port:** `5678` (default n8n dashboard interface port)

---

## ⚙️ How to Build & Run

### 1. Build the Docker Image
```bash
docker build -t n8n-birthday-bot .
```

### 2. Run the Container
```bash
docker run -d --name n8n-bot -p 5678:5678 n8nio/n8n:latest
```
Access the dashboard at `http://localhost:5678/` to configure scheduling nodes and integrations.

---

## 📄 License

Licensed under the MIT License. See [LICENSE](LICENSE) for details.
