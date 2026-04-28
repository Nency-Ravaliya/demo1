# Docker Commands Cheat Sheet (Beginner Friendly)

## What is Docker?
Docker helps you run applications in containers so they work the same everywhere.

---

## Basic Docker Workflow
Write Code → Create Dockerfile → Build Image → Run Container

---

## 1. Check Docker Version
```bash
docker --version
```
Check if Docker is installed properly

---

## 2. Pull Image from Docker Hub
```bash
docker pull nginx
```
Download an existing image from internet

---

## 3. View Downloaded Images
```bash
docker images
```
List all images on your system

---

## 4. Build Docker Image
```bash
docker build -t my-website .
```
Create your own image using Dockerfile

---

## 5. Run Container
```bash
docker run -d -p 80:80 my-website
```
Run container in background and map port

---

## 6. View Running Containers
```bash
docker ps
```
See all running containers

---

## 7. View All Containers
```bash
docker ps -a
```
See running and stopped containers

---

## 8. Stop Container
```bash
docker stop <container-id>
```
Stop a running container

---

## 9. Start Container
```bash
docker start <container-id>
```
Start a stopped container

---

## 10. Remove Container
```bash
docker rm <container-id>
```
Delete a container

---

## 11. Remove Image
```bash
docker rmi <image-id>
```
Delete an image

---

## 12. Run Container with Name
```bash
docker run -d -p 80:80 --name myapp my-website
```
Run container with custom name

---

## 13. Check Container Logs
```bash
docker logs <container-id>
```
View logs of container

---

## 14. Execute Command Inside Container
```bash
docker exec -it <container-id> /bin/bash
```
Access container terminal

---

## 15. Stop All Containers
```bash
docker stop $(docker ps -q)
```
Stop all running containers

---

## 16. Remove All Containers
```bash
docker rm $(docker ps -aq)
```
Delete all containers

---

## 17. Remove All Images
```bash
docker rmi $(docker images -q)
```
Delete all images

---

## Quick Summary
Dockerfile → Build → Image → Run → Container


