# 🎮 Game 2048 - Dockerized Version

A classic 2048 browser-based game, containerized using Docker and deployed to AWS Elastic Beanstalk.

---

## 📦 Project Description

This project packages the original [2048 game](https://github.com/gabrielecirulli/2048) inside a lightweight **Docker container** using **Nginx** as a web server. It’s a fully functional, containerized static site ready for deployment on any cloud platform.

---

## 🌐 Live Demo

👉 [Play the Game Here](http://2048-env.eba-5ub7akqw.ap-south-1.elasticbeanstalk.com/)

---

## 🐳 Docker Setup

### 🔨 Build the Docker Image

```bash
docker build -t game-2048 .
```

---

docker run -d -p 7071:80 game-2048

---
