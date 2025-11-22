

<h1> **MERN**, **DevOps**, **Backend**, **Microservices**, **Cloud**, and **Deployment**</h1>

---

# 🚀 **1. Docker Basics**

```
docker --version
docker info
docker help
```

---

# 🚀 **2. Docker Images (Very Important)**

```
docker images                      → List images
docker pull <image>                → Download image
docker rmi <image>                 → Delete image
docker tag <image> <newname>       → Rename/tag image
docker build -t <name> .           → Build image from Dockerfile
docker save -o file.tar <image>    → Save image to tar file
docker load -i file.tar            → Load image from tar
```

---

# 🚀 **3. Docker Containers**

```
docker ps                         → Running containers
docker ps -a                      → All containers
docker run <image>                → Run container
docker run -d <image>             → Run in background
docker run -p 3000:3000 <image>   → Port mapping
docker run -it <image> bash       → Open terminal inside container
docker start <id>                 → Start stopped container
docker stop <id>                  → Stop container
docker restart <id>               → Restart container
docker kill <id>                  → Kill container immediately
docker rm <id>                    → Remove container
docker commit <container> <image> → Create image from container
```

---

# 🚀 **4. Logs & Debugging**

```
docker logs <id>                  → Show logs
docker logs -f <id>               → Follow logs (live)
docker exec -it <id> bash         → Enter container terminal
docker inspect <id>               → Detailed info
docker diff <id>                  → Show file changes inside container
```

---

# 🚀 **5. Networks (Important for Microservices)**

```
docker network ls                     → List networks
docker network create <name>          → Create network
docker network connect <net> <cont>   → Attach container to network
docker network disconnect <net> <cont>
docker network inspect <net>
```

---

# 🚀 **6. Volumes (Data Persistence)**

```
docker volume ls                   → List volumes
docker volume create <name>        → Create volume
docker volume inspect <name>
docker volume rm <name>            → Delete volume
docker volume prune                → Delete unused volumes
```

---

# 🚀 **7. Docker Compose (Used in all real DevOps setups)**

### **Basic commands**

```
docker compose up
docker compose up -d
docker compose down
docker compose down --volumes
docker compose restart
docker compose logs
docker compose logs -f
docker compose ps
```

### **Rebuild**

```
docker compose up --build
docker compose build
```

### **Execute inside a compose service**

```
docker compose exec <service> bash
```

---

# 🚀 **8. Docker Cleanup Commands (must know)**

```
docker system df                     → Disk usage
docker system prune                  → Cleanup unused data
docker system prune -a               → Remove unused images/containers
docker rm $(docker ps -aq)           → Remove all containers
docker rmi $(docker images -q)       → Remove all images
```

---

# 🚀 **9. Docker Registry**

```
docker login
docker logout
docker push <image>
docker pull <image>
```

---

# 🚀 **10. Dockerfile Commands (Used to build images)**

```
FROM
RUN
COPY
ADD
WORKDIR
EXPOSE
CMD
ENTRYPOINT
ENV
USER
VOLUME
```

---
