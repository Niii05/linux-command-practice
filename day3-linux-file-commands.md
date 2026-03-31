# Day 3 - Docker + Nginx Basics

## 🧠 What I Learned

### 1. Docker Run Command

```bash
docker run -d -p 8080:80 nginx
```

* `docker run` → creates and starts container
* `-d` → runs container in background
* `-p 8080:80` → maps host port 8080 to container port 80
* `nginx` → image used to run web server

---

### 2. Port Mapping

```
Host (8080) → Container (80)
```

* Browser sends request to `localhost:8080`
* Docker forwards it to container port `80`
* Nginx handles the request

---

### 3. Foreground vs Background

Without `-d`:

* Terminal gets blocked
* Logs are visible

With `-d`:

* Container runs in background
* Terminal is free

---

### 4. Checking Containers

```bash
docker ps
```

* Shows running containers

```bash
docker ps -a
```

* Shows all containers

---

### 5. Stopping and Removing Containers

```bash
docker stop <container_id>
docker rm <container_id>
```

Shortcut:

```bash
docker rm -f <container_id>
```

---

### 6. Accessing Nginx

Open in browser:

```
http://localhost:8080
```

* Displays "Welcome to nginx!" page

---

### 7. Key Concepts

* Container = isolated environment
* Docker = runs containers
* Nginx = web server
* Port mapping = connection between host and container

---

## 🚀 Summary

Docker allows running applications inside containers.
Using port mapping, we can access container services from our local system.
