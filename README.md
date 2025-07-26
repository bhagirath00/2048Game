# Game-2048 — Dockerized Web App 🎮

A minimal, containerized version of the legendary **2048** browser game. Built with **Docker**, served with **Nginx**, and deployed to **AWS Elastic Beanstalk**.

🔗 <a href="http://2048-env.eba-5ub7akqw.ap-south-1.elasticbeanstalk.com/" target="_blank"><strong>Live Demo</strong></a>

---

## 📌 Project Overview

This project Dockerizes the original [2048 game](https://github.com/gabrielecirulli/2048) using a production-ready Nginx setup. It demonstrates how to serve a static web app using Docker and deploy it seamlessly to AWS.

---

## Tech Stack

| Tool/Service             | Purpose                       |
| ------------------------ | ----------------------------- |
| 🐳 Docker                | Containerization              |
| 🌐 Nginx                 | Static file web server        |
| 🐧 Ubuntu 22.04          | Lightweight base image        |
| ☁️ AWS Elastic Beanstalk | Production deployment         |
| 🔧 curl, zip             | Game fetch & setup automation |

---

## 💡 Why This Project?

This project was built to learn and showcase Dockerized deployments of static web applications.
It serves as a foundational DevOps example using Nginx, Docker, and AWS.

---

## How to Run Locally

### Step 1: `Build the Docker Image`

```bash
docker build -t game-2048 .
```

---

### Step 2: `Run the Container`

```bash
docker run -d -p 7071:80 game-2048
```

---

📂 File Structure

```plaintext
game-2048/
├── Dockerfile       # Defines how to build the container
├── assets/          # Optional: screenshots, logos
└── README.md        # This documentation
```

---

🐳 Dockerfile Breakdown

```plaintext
- Installs required dependencies
- Downloads and unzips the 2048 game
- Configures Nginx to serve it on port 80
```

---

☁️ Deployment (AWS Elastic Beanstalk)

```plaintext
Deployed using:
- Elastic Beanstalk Docker environment
- Single-container Docker deployment via AWS Console
```

🔗 Live App: http://2048-env.eba-5ub7akqw.ap-south-1.elasticbeanstalk.com/

---

⭐️ Support

```plaintext
If you found this helpful or learned something, please consider giving this repo a ⭐️
— it helps others discover the project and supports my work.

```

---
