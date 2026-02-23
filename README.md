# 🤖 Telegram Groq Chatbot

A powerful, context-aware Telegram chatbot powered by **Groq** and the **Llama-3.3-70b-versatile** model. This bot maintains conversation history and provides lightning-fast responses.

---

## 🚀 Features

- **Blazing Fast AI**: Powered by Groq's LPUs for near-instant responses.
- **Context Retention**: Remembers the previous turn in the conversation for more coherent interactions.
- **Easy Management**: Simple commands to reset context or get help.
- **Docker Ready**: Fully containerized for easy deployment.

## 🛠️ Tech Stack

- **AI SDK**: [Groq Python SDK](https://github.com/groq/groq-python)
- **Bot Framework**: [Aiogram 2.x](https://github.com/aiogram/aiogram)
- **Environment Management**: `python-dotenv`
- **Language**: Python 3.8+

## 📋 Commands

- `/start` - Initialize the bot and get a welcome message.
- `/help` - View the help menu and available commands.
- `/clear` - Clear the current conversation context/history.
- `ANY TEXT` - Send any message to receive an AI-generated response.

---

## ⚙️ Setup & Installation

### 1. Clone the Repository
```bash
git clone <repository-url>
cd <project-directory>
```

### 2. Create a Virtual Environment
```bash
python -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

### 4. Configure Environment Variables
Create a `.env` file in the root directory and add your credentials:
```env
TELEGRAM_BOT_TOKEN="your_telegram_bot_token"
GROQ_API_KEY="your_groq_api_key"
```
> [!TIP]
> Get your Telegram token from [@BotFather](https://t.me/botfather) and your Groq API key from the [Groq Console](https://console.groq.com/keys).

---

## 🏃 Running the Bot

### Locally
```bash
python main.py
```

### Using Docker
1. **Build the Image**:
   ```bash
   docker build -t telegram-groq-bot .
   ```
2. **Run the Container**:
   ```bash
   docker run --rm --env-file .env telegram-groq-bot
   ```

---

## 📄 License

This project is licensed under the [MIT License](LICENSE). 
Copyright (c) 2026 BAPPY AHMED.

---

*Created with ❤️ by BAPPY AHMED.*
