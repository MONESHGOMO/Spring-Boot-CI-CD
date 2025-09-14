# Spring Boot App with Docker & GitHub Actions

This repository contains a simple Spring Boot application packaged with **Docker** and built/pushed automatically using **GitHub Actions**.  
The app runs on **port 8089** inside the container.

---

## 🚀 How to Build & Run Locally

### 1. Build the Docker image
```bash
docker build -t moneshgomo/springboot-image-github-actions .
```

### 2. Run the container
```bash
docker run -d -p 8089:8089 --name springboot-container moneshgomo/springboot-image-github-actions
```
- `-d` → run in background  
- `-p 8089:8089` → maps container port 8089 to your host  
- `--name springboot-container` → gives your container a custom name  

### 3. Access the app
Open your browser and go to:  
👉 [http://localhost:8089](http://localhost:8089)

---

## 🐳 Docker Commands

**Stop the container:**
```bash
docker stop springboot-container
```

**Start it again:**
```bash
docker start springboot-container
```

**View logs:**
```bash
docker logs -f springboot-container
```

**Remove the container:**
```bash
docker rm -f springboot-container
```
