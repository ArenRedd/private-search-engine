# 🔍 Private Search Engine – 70 Engines in One

Welcome to your self-hosted, privacy-focused meta search engine — powered by [SearXNG](https://github.com/searxng/searxng) and Docker. This engine pulls search results from **70+ search engines simultaneously**, giving you a fast, ad-free, and surveillance-free browsing experience.

> 💡 Bonus: Integrate with LLaMA 2 and Ollama for private AI-powered interactions.

---

## 🚀 Features

- 🔐 **Privacy First** – No tracking, no ads, and no user profiling.
- 🛠️ **Fully Customizable** – Choose your preferred engines, UI, and filters.
- 🌍 **Meta Search** – Fetches results from multiple search engines in parallel.
- 🤖 **AI Integration Ready** – Connect with private LLaMA 2 via Ollama.
- 💻 **Self-Hosted** – Complete control over your infrastructure.
- 🔌 **Extensible** – Easily integrate with private cloud or file storage solutions.

---

## 🧠 Architecture Overview

![Architecture Diagram](https://res.cloudinary.com/dke6ddkot/image/upload/v1748709351/search-engine-architecture_jxcdoh.png)

📂 Project Structure
```bash
/usr/local/searxng-docker/
├── searxng/
│   ├── docker-compose.yml
│   ├── .env
│   └── ... (other configs & scripts)
```
⚙️ Installation
1. 📥 Clone the Repository
```bash
git clone https://github.com/<your-username>/private-search-engine.git
cd private-search-engine/searxng
```
2. 🔧 Configure (Optional)
Edit settings.yml inside the searxng folder to customize:

Enabled search engines

Result categories

UI themes

Safe search filters

3. 🐳 Start the Search Engine
```bash
sudo docker-compose up -d
```
This will start the engine and make it available at:
```cpp
http://192.168.1.4:8888
```
⛔ Stopping the Server
To shut down the search engine:

```bash
sudo docker-compose down
```
🧠 AI Integration Prompt (for LLaMA 2 via Ollama)
If you're using this search engine in conjunction with a private LLaMA 2 chatbot, you can integrate results using the following context prompt:

🧠 Prompt Template
"You are a private AI assistant connected to a self-hosted meta search engine. Search results are pulled from 70 sources without censorship or tracking. Use this information to answer the user's question with accuracy and independence, citing results where needed."

Example usage in Ollama:
```bash
ollama run llama2
```
Prompt inside the chat:

```pgsql
You have access to a private search engine hosted at http://192.168.1.4:8888. Search for "latest zero-day vulnerabilities in 2025" and summarize the top results.
```
🔐 Use Cases
Security research (ad-free, uncensored)

Academic learning (no distractions)

Private personal assistant (LLaMA 2 + Ollama + SearXNG)

Offline or LAN-only usage

Integration with home cloud storage

📎 Related Projects
SearXNG GitHub

Ollama

LLaMA 2

Docker

🧑‍💻 Maintainer
AnandRam Mohan (aka Aren Redd)
Blog • GitHub

🪪 License
This project is licensed under the MIT License.

