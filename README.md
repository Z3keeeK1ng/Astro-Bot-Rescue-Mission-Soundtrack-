<div align="center">

# 🤖 AstrBot

**An open-source, all-in-one Agent chatbot platform for mainstream instant messaging apps.**

[![GitHub Stars](https://shields.io)](https://github.com/AstrBotDevs/AstrBot)
[![Documentation](https://shields.io)](https://docs.astrbot.app)
[![License](https://shields.io)](https://github.com/AstrBotDevs/AstrBot)

[Documentation](https://docs.astrbot.app) • [Plugin Development](https://docs.astrbot.app/en/dev/star/plugin-new.html) • [Issue Tracker](https://github.com)

</div>

---

## 📖 Overview

**AstrBot** provides reliable, scalable conversational AI infrastructure for individuals, developers, and teams. Whether you are building a personal AI companion, intelligent customer service, workflow automation, or an enterprise knowledge base, AstrBot enables you to deploy production-ready AI agents directly into your favorite messaging platforms.

## ✨ Key Features

* **Multi-Platform IM Integration:** Seamlessly connect your AI agent to Telegram, Discord, Slack, WeChat, QQ, and more.
* **Multi-LLM & Embedding Support:** Compatible with OpenAI-compatible APIs, Google Gemini, DeepSeek, Ollama (local models), Alibaba Cloud Model Studio, and NVIDIA.
* **Built-in RAG Knowledge Base:** Upload product manuals, FAQs, or project documentation so your agent can retrieve relevant context without fine-tuning.
* **Extensive Plugin Ecosystem:** Access 1,000+ community plugins with one-click installation, or build your own in Python using the AstrBot Plugin SDK.
* **Agentic Capabilities:** Features built-in web search, sandboxed code execution, sub-agent orchestration, context compression, and proactive messaging.
* **Visual WebUI:** Manage providers, personas, knowledge bases, permissions, and plugin configurations through an intuitive web dashboard.

---

## 🚀 Quick Start

### Option 1: Deploy with Docker (Recommended)
Run AstrBot in an isolated container with a single command:

```bash
docker run -itd \
  --name astrbot \
  -p 6180-6200:6180-6200 \
  -v \$(pwd)/data:/AstrBot/data \
  soulter/astrbot:latest
```

### Option 2: Run from Source (using `uv` or `pip`)
1. **Clone the repository:**
   ```bash
   git clone https://github.com
   cd AstrBot
   ```
2. **Install dependencies and start:**
   ```bash
   uv run main.py
   # Or using standard Python:
   # pip install -r requirements.txt && python main.py
   ```
3. **Access the WebUI:** Open `http://localhost:6185` in your browser to configure your LLM provider and messaging platform adapters.

---

## 🧩 Plugin Development

Want to extend AstrBot with custom commands or AI tools? Plugins follow a simple structure (`astrbot_plugin_<name>`):

1. Place your plugin folder inside `data/plugins/<plugin-directory>/`.
2. Define your plugin details in `metadata.yaml`.
3. Write your event listeners or LLM tools in Python and hot-reload directly from the **WebUI**.

👉 Check out the [AstrBot Plugin Development Guide](https://docs.astrbot.app/en/dev/star/plugin-new.html) for full API references.

---

## 🤝 Contributing & Support

* **Bug Reports & Feature Requests:** Open an issue on the [GitHub Issue Tracker](https://github.com).
* **Community:** Join the developer community to share personas, plugins, and deployment tips.

---

<div align="center">
  <sub>Built with ❤️ by the <a href="https://github.com/AstrBotDevs">AstrBot</a> community.</sub>
</div>
