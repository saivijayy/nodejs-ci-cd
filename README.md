# 🚀 Node.js CI/CD Pipeline using GitHub Actions & Docker

## 📌 Task Overview

This project is a part of my DevOps Internship – **Task 1: Automate Code Deployment Using CI/CD Pipeline**.  
The goal was to set up a CI/CD pipeline using **GitHub Actions** to build and deploy a sample **Node.js** web app using **Docker** and **DockerHub**.

---

## 🛠️ Tech Stack

- Node.js
- Docker
- GitHub Actions
- DockerHub

---

## 📂 Project Structure

```
.
├── Dockerfile
├── app.js
├── bin/
├── public/
├── routes/
├── views/
├── package.json
├── .github/
│   └── workflows/
│       └── main.yml
```

---

## ⚙️ CI/CD Workflow

The CI/CD pipeline is defined in `.github/workflows/main.yml`.

### ✅ What It Does:
1. Triggers on **push to the `main` branch**
2. Installs dependencies (`npm install`)
3. Runs test script (`npm test`)
4. Builds Docker image
5. Pushes image to **DockerHub** (`saivjayy/express-cicd-app`)

---

## 🐳 DockerHub Link

> 🔗 [https://hub.docker.com/r/saivjayy/express-cicd-app](https://hub.docker.com/r/saivjayy/express-cicd-app)

---

## 🧪 Local Run

```bash
# Build image
docker build -t express-cicd-app .

# Run container
docker run -p 3000:3000 express-cicd-app
```

Then open: [http://localhost:3000](http://localhost:3000)

---

## 📚 What I Learned

- How GitHub Actions automates CI/CD pipelines
- Writing YAML workflows
- Dockerizing a Node.js app
- Pushing to DockerHub
- Automating tests, builds, and deploys

---

## 📁 Submission

✅ Task completed and submitted as per the internship guidelines.

---

