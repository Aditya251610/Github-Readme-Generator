# 🛠️ GitHub Repo Auto-Documentation Workflow using n8n + Local AI

This project provides an **n8n workflow** that automatically generates a professional README file for any public GitHub repository using AI models like Ollama or Groq.

---

## ✅ Features

- 🌐 User submits a **GitHub repository URL**
- 📂 **Fetches all files** recursively, excluding sensitive files like `.env`
- 🤖 Feeds file content to a **locally hosted AI model**
- 📝 AI writes a **clean, detailed README.md** based on project structure and code analysis
- 💻 Easy to self-host using **Docker**

---

## 📂 Files in This Repository

- `My workflow 2.json`:  
  The n8n workflow export file. Import this into your n8n instance to get started.

---

## 🚀 How to Use

### 1️⃣ Setup n8n

Use either:
- [n8n Cloud](https://n8n.io/)
- Self-hosted via Docker:
  
  ```bash
  docker run -it --rm \
    -p 5678:5678 \
    -v ~/.n8n:/home/node/.n8n \
    n8nio/n8n
