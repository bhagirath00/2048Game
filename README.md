<!-- # 🎮 Game 2048 - Dockerized Version

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

--- -->

---

```markdown
<h1 align="center">🎮 Game 2048 — Dockerized Web App</h1>

<p align="center">
  A minimal, containerized version of the legendary <b>2048</b> browser game. Built with <b>Docker</b>, served with <b>Nginx</b>, and deployed to <b>AWS Elastic Beanstalk</b>.
</p>

<p align="center">
  <a href="http://2048-env.eba-5ub7akqw.ap-south-1.elasticbeanstalk.com/" target="_blank">
    🔗 <b>Live Demo</b>
  </a>
</p>

---

## 📌 Project Overview

This project Dockerizes the original [2048 game](https://github.com/gabrielecirulli/2048) using a production-ready Nginx setup. It demonstrates how to serve a static web app using Docker and deploy it seamlessly to AWS.
```

---

## 🧰 Tech Stack

| Tool/Service             | Purpose                       |
| ------------------------ | ----------------------------- |
| 🐳 Docker                | Containerization              |
| 🌐 Nginx                 | Static file web server        |
| 🐧 Ubuntu 22.04          | Lightweight base image        |
| ☁️ AWS Elastic Beanstalk | Production deployment         |
| 🔧 curl, zip             | Game fetch & setup automation |

---

## 🛠️ How to Run Locally

### 🔨 Step 1: Build the Docker Image

```bash
docker build -t game-2048 .
```

````

### 🚀 Step 2: Run the Container

```bash
docker run -d -p 7071:80 game-2048
```

Open in browser: [http://localhost:7071](http://localhost:7071)

---

## 📂 File Structure

```
game-2048/
├── Dockerfile       # Defines how to build the container
├── .gitignore       # Files to exclude from Git
├── README.md        # This documentation
└── assets/          # Optional: screenshots, logos
```

---

## 🐳 Dockerfile Explanation

```dockerfile
FROM ubuntu:22.04

RUN apt-get update && \
    apt-get install -y nginx zip curl && \
    echo "daemon off;" >> /etc/nginx/nginx.conf && \
    curl -o /var/www/html/master.zip -L https://codeload.github.com/gabrielecirulli/2048/zip/master && \
    cd /var/www/html/ && unzip master.zip && mv 2048-master/* . && rm -rf 2048-master master.zip

EXPOSE 80
CMD ["/usr/sbin/nginx", "-c", "/etc/nginx/nginx.conf"]
```

- ✅ Installs required dependencies
- ✅ Downloads and unzips the 2048 game
- ✅ Configures Nginx to serve it on port 80

---

## ☁️ Deployment (AWS Elastic Beanstalk)

Deployed using:

- Elastic Beanstalk Docker environment
- Single-container Docker deployment via AWS Console

🟢 [Live App Link](http://2048-env.eba-5ub7akqw.ap-south-1.elasticbeanstalk.com/)

---

## 📸 Screenshots (Optional)

> Place images in `assets/` folder and embed below:

```markdown
<p align="center">
  <img src="assets/screenshot-local.png" width="600" alt="Game running locally">
  <br/>
  <i>Running locally on Docker (localhost:7071)</i>
</p>
```

---

## 👨‍💻 Author

**Patel Bhagirath Dungaram**
📧 \[Your Email Here]
🔗 \[GitHub / LinkedIn profile link]

---

## 🙌 Acknowledgements

- [Gabriele Cirulli](https://github.com/gabrielecirulli) — Creator of the original 2048 game.
- [Docker](https://www.docker.com/) — For containerization.
- [AWS Elastic Beanstalk](https://aws.amazon.com/elasticbeanstalk/) — For cloud deployment.

---

## ⭐️ Support

If you found this helpful or learned something, please consider giving this repo a ⭐️! It helps others discover the project and keeps me motivated.

```

---

### 💡 Bonus Suggestions

If you want to take it even further:
- Add badges (e.g. Docker Pulls, GitHub stars)
- Add a demo video GIF (e.g., recorded via Screenity or OBS)
- Use a custom domain via AWS Route 53

---
````
