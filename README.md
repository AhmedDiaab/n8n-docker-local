# n8n Docker Local Setup

This repository contains a simple setup to run the **n8n (Community Edition)** workflow automation tool locally using Docker Compose.

## 🚀 Getting Started

### 1. Clone the repo

```bash
git clone https://github.com/your-username/n8n-docker-local.git
cd n8n-docker-local
```

### 2. Create `.env` file

```env
# .env
N8N_BASIC_AUTH_ACTIVE=true
N8N_BASIC_AUTH_USER=admin
N8N_BASIC_AUTH_PASSWORD=admin
N8N_HOST=localhost
N8N_PORT=5678
N8N_PROTOCOL=http
NODE_ENV=production
```

> ⚠️ Change the default credentials for security!

### 3. Start the services

```bash
docker-compose --env-file .env up -d
```

### 4. Access n8n

Visit: [http://localhost:5678](http://localhost:5678)  
Login: `admin` / `admin`

## 📁 Project Structure

```
n8n-docker-local/
├── docker-compose.yml
└── .env
```

## 🛠 Features

- Persistent data volume
- Basic authentication
- Easily extendable (e.g., Postgres, webhook exposure, reverse proxy)

## 📄 License

MIT