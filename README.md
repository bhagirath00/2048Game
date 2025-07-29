# Game-2048 🎮

A Dockerized version of the legendary 2048 browser game, served using Nginx Alpine.

![2048 Game running locally](assets/image-1.png)

## Run Instantly (Docker Hub)

You can pull and run the game directly from Docker Hub without building anything:

```bash
docker run -d -p 7071:80 bhagirath00/game-2048:latest
```

Open your browser and navigate to: **[http://localhost:7071](http://localhost:7071)**

---

## Run Locally (Build from Source)

If you want to build and run the image locally:

### 1. Build the Docker Image
```bash
docker build -t game-2048:latest .
```

### 2. Run the Container
```bash
docker run -d -p 7071:80 game-2048:latest
```
