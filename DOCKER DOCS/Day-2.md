# 🐳 Day 2: Docker Images vs Containers

---

## ✅ Goals for Today
1. Understand the difference between **Images** and **Containers**
2. Learn common commands to work with both
3. Explore container lifecycle and inspect running containers

---

## 📦 1. What is a Docker Image?

- A **Docker Image** is like a **blueprint** or **snapshot**.
- It’s **read-only** and contains everything your app needs to run:
  - Code
  - Libraries
  - Environment variables
  - System tools

Think of it like a `.zip` file or ISO image of your app.

You create images using a **Dockerfile**.

---

## 📦 2. What is a Docker Container?

- A **Container** is a **running instance** of an image.
- It’s **read-write**, isolated, and has its own filesystem and network.
- You can run multiple containers from the same image.

---

### 🧠 Analogy:

| Concept       | Analogy             |
|---------------|---------------------|
| **Image**     | Recipe              |
| **Container** | Cooked dish         |

---

## 🔧 3. Common Commands

### 🔍 View all images on your system:
```bash
docker images
```

### ▶️ Run a container from an image:
```bash
docker run ubuntu echo "Hello from Ubuntu"
```

### 📋 View running containers:
```bash
docker ps
```

### 📜 View all containers (even stopped ones):
```bash
docker ps -a
```

### 🛑 Stop a running container:
```bash
docker stop <container-id>
```

### 🧽 Remove a container:
```bash
docker rm <container-id>
```

### 🧼 Remove an image:
```bash
docker rmi <image-id>
```

---

## 🔎 4. Container Lifecycle

A container goes through these stages:

1. **Created**
2. **Running**
3. **Stopped**
4. **Removed**

Example:
```bash
docker run -d --name demo-container nginx
docker stop demo-container
docker rm demo-container
```

---

## 🧠 5. Key Differences: Image vs Container

| Feature         | Docker Image           | Docker Container           |
|-----------------|------------------------|----------------------------|
| Type            | Blueprint              | Running instance           |
| Mutability      | Immutable (read-only)  | Mutable (read-write)       |
| Status          | Stored on disk         | Running in memory (or stopped) |
| Command         | `docker build`         | `docker run`               |

---

## 📝 Homework (Optional)

1. Run a container and explore it interactively:
```bash
docker run -it ubuntu bash
```
Then try:
```bash
ls
pwd
exit
```

2. Stop and remove containers/images you created:
```bash
docker ps -a
docker stop <id>
docker rm <id>
docker images
docker rmi <id>
```

---

✅ That’s it for **Day 2**! You now understand the **heart of Docker** — images and containers.
