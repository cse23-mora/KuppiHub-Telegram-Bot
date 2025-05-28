# 🤖 Official Telegram Bot – Kuppihub

> This is a demo. We’ve modified some features for our purposes.



## 🚀 Features

- 📤 Upload any **video**, **photo**, **audio**, or **document** (up to 4GB)
- 📬 Get a **Telegram shareable link**

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
