# 📄 GitHub Repo Doc Generation Workflow (n8n)

Generate structured, professional README.md files automatically by analyzing all files in a public GitHub repository using n8n and an AI agent.

---

## 🚀 Features

- Analyze all files in a public GitHub repository recursively
- Automatically generate a README.md file based on actual code and project structure
- Works with:
  - Ollama (local AI models)
  - Groq API or OpenAI API (cloud AI models)
- Uses n8n workflow automation platform
- Works with Docker or n8n Cloud

---

## 🎯 How to Use

### 🛠️ Setup n8n

Use either:

- [n8n Cloud](https://n8n.io/)
- Self-hosted via Docker:

```bash
docker run -it --rm \
  -p 5678:5678 \
  -v ~/.n8n:/home/node/.n8n \
  n8nio/n8n

📥 Import the Workflow

    Go to n8n → Workflows → Import Workflow

    Upload My workflow 2.json from this repository.

🤖 Set Up AI Integration

    Host Ollama locally:

ollama serve

    Or use Groq/OpenAI API and update HTTP Request node in n8n accordingly.

🌐 Provide Your GitHub Repo URL

Send a POST request to the Webhook trigger in n8n:

{
  "repo_url": "https://github.com/your-username/your-repo"
}

You’ll receive a structured, AI-generated README file as the response.
🛠️ Technologies Used

    n8n

    Ollama or Groq

    PostgreSQL (optional for workflow state/history)

    Docker

📢 Contributing & Feedback

If you find this workflow helpful:

    ⭐ Star this repo

    ✅ Fork and contribute ideas

    💬 Connect with me on LinkedIn

📸 Screenshot Preview

Upload your workflow screenshot here if you want.
Example:

<img width="1281" height="256" alt="image" src="https://github.com/user-attachments/assets/019110ba-4fd7-489e-b05c-cc54d9038090" />



⚠️ Notes

    Only public GitHub repositories are supported.

    Sensitive files like .env are automatically excluded.

    Be mindful of API limits when using cloud AI services like OpenAI or Groq.
