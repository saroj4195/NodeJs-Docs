# 🐳 Day 1: Introduction to Docker

## ✅ Goals for Today:
1. Understand what Docker is.
2. Install Docker.
3. Run your first Docker container (`hello-world`).
4. Learn basic Docker terminology.

---

## 🔁 1. What is Docker?

- Docker is a tool that lets you **package your app and its dependencies into containers**.
- Containers work on any system with Docker installed.
- It solves the "it works on my machine" problem.

---

## 💻 2. Install Docker

Go to: [https://www.docker.com/products/docker-desktop](https://www.docker.com/products/docker-desktop)

### Installation Steps (Windows/Mac):
1. Download Docker Desktop.
2. Install and reboot if needed.
3. Open Docker Desktop.
4. Open a Terminal (Mac/Linux) or Command Prompt (Windows).

---

## 🔍 3. Verify Docker Installation

Run this command:
```bash
docker --version
```

You should see output like:
```
Docker version 25.0.0, build abc123
```

If yes, Docker is installed successfully!

---

## ✅ 4. Run Your First Container

```bash
docker run hello-world
```

### What this does:
- Downloads the `hello-world` image from Docker Hub (if not present).
- Creates a container from that image.
- Runs it and prints a success message.

### Expected Output:
```
Hello from Docker!
This message shows that your installation appears to be working correctly.
```

---

## 🧠 5. Key Docker Terms

| Term           | Description                                   |
|----------------|-----------------------------------------------|
| **Image**      | A read-only blueprint of your application.    |
| **Container**  | A running instance of an image.               |
| **Dockerfile** | A set of instructions to build an image.      |
| **Docker Hub** | A repository of Docker images.                |

---

## 📝 Homework (Optional)

1. Visit [https://hub.docker.com](https://hub.docker.com)
2. Search for images like:
   - `ubuntu`
   - `nginx`
   - `mysql`
   - `python`
3. Try this:
```bash
docker run ubuntu echo "Hi from Ubuntu"
```

---

✅ Congratulations! You’ve completed **Day 1** of Docker learning!

