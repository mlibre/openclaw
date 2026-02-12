# 🦞 OpenClaw AI Automation Tool

OpenClaw is an AI-powered automation tool that provides a web interface for interacting with AI models through a unified gateway.

## 🚀 Features

- 🤖 Unified AI model gateway
- 🌐 Web interface with password protection
- 💬 Telegram integration
- 📝 Workspace management
- 🎯 Agent orchestration
- 🔌 Plugin support

## 📦 Installation

### Prerequisites

- Node.js (16.x or higher)
- Render.com account
- AI model provider (e.g., LocalAI)
- Telegram bot token (optional but recommended)

### Deployment on Render

1. **Create a remote repository** on GitHub or GitLab and push this code

2. **Deploy on Render.com:**
   - Go to [Render.com](https://render.com) and create a new **Web Service**
   - Connect your GitHub/GitLab repository
   - Configure the deployment:
     - **Runtime:** Node
     - **Build Command:** `npm install`
     - **Start Command:** `npm start`

3. **Set Environment Variables:**
   Add these environment variables in Render's dashboard:

   | Variable                        | Value                | Description                   |
   | ------------------------------- | -------------------- | ----------------------------- |
   | `OPENCLAW_GATEWAY_PASSWORD`     | `your_secure_pass`   | Protects your public UI       |
   | `MODEL_API_KEY`                 | `provider-api-key`   | AI Provider API token         |
   | `MODEL_BASE_URL`                | `provider-base-url`  | AI Provider Base URL          |
   | `OPENCLAW_TELEGRAM_TOKEN`       | `telegram-bot-token` | Telegram Bot (optional)       |
   | `OPENCLAW_STATE_DIR` (optional) | `/var/data`          | Where to save sessions/logins |

## 🎮 Usage

Once deployed:

1. Visit your Render service URL
2. Enter the password you set for `OPENCLAW_GATEWAY_PASSWORD`
3. Start interacting with AI models through the web interface
