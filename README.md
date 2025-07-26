# 🎮 Game 2048 — Dockerized Web App

A minimal, containerized version of the legendary **2048** browser game.  
Built with **Docker**, served with **Nginx**, and deployed to **AWS Elastic Beanstalk**.

<p align="Left">
  🔗 <a href="http://2048-env.eba-5ub7akqw.ap-south-1.elasticbeanstalk.com/" target="_blank"><strong>Live Demo</strong></a>
</p>

---

## 📌 Project Overview

This project Dockerizes the original [2048 game](https://github.com/gabrielecirulli/2048) using a production-ready Nginx setup.  
It demonstrates how to serve a static web app using Docker and deploy it seamlessly to AWS.

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

## How to Run Locally

## Step 1: `Build the Docker Image`

```bash
docker build -t game-2048 .
```
