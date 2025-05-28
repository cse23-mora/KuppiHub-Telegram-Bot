# 🤖 Official Telegram Bot Kuppihub

Hi there! I'm **KupppiHub Telegram  Bot**, a powerful Telegram bot  helps users convert any file into a **direct download link**, **stream link**, and a **Telegram shareable link**. ✨

---

## 🚀 Features

- 📤 Upload any **video**, **photo**, **audio**, or **document** (up to 4GB)
- 🔗 Get a **direct download link**
- 📺 Get a **stream link** for files under 20MB
- 📬 Get a **Telegram shareable link**
- 💡 No need for your friends to have Telegram to access files!

---

## 🛠 Setup Instructions

Follow these steps to deploy the bot using **Cloudflare Workers**:

### 1️⃣ Clone this repo
```bash
git clone https://github.com/your-username/KupppiHub Telegram  Bot-link-bot.git
```

### 2️⃣ Replace the following values in `workers.js`:

```javascript
const BOT_TOKEN = "";        // 👉 Your Telegram Bot Token
const BOT_SECRET = "secret"; // 👉 A secure random string
const BOT_CHANNEL = ;        // 👉 Your Telegram Channel ID (as an integer)
const SIA_NUMBER = 1234;     // 👉 A random secret integer (same across bot & backend)
const BOT_OWNER = "YourUserName"; // 👉 Your Telegram username (for /start button)
```

> 📝 Make sure your bot is added as an admin in your channel.

---

### 3️⃣ Deploy on Cloudflare Workers

1. Copy-paste the `workers.js` file into the [Cloudflare Workers editor](https://dash.cloudflare.com/)
2. Save and deploy the worker.

---

### 4️⃣ Register Webhook

Go to:
```
https://your-domain.com/registerWebhook
```

✅ If everything is okay, it will return:
```json
{"ok":true,"result":true,"description":"Webhook was set"}
```

Your bot is now live and ready to use!

---
