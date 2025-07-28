# ChatGPT Voice UI — Backend

This is the Node.js + Express backend for the ChatGPT Voice web app.  
It accepts a message from the frontend, sends it to ChatGPT via OpenAI API (or OpenRouter), and returns the reply.

---

## 🧠 Features

- Receives messages from frontend
- Sends request to ChatGPT API (via OpenAI SDK or OpenRouter)
- Returns reply to client
- Built-in error handling

---

## ⚙️ Tech Stack

- [Node.js](https://nodejs.org/)
- [Express](https://expressjs.com/)
- [OpenAI SDK](https://www.npmjs.com/package/openai) (or use fetch + OpenRouter)

---

## 📦 Installation & Usage

`bash
npm install
node server.js

Runs on: http://localhost:5000


---

🔐 Environment Variables

Create a .env file with your API key:

OPENAI_API_KEY=your-api-key-here

> ✅ Optional: if using OpenRouter, replace endpoint and use OPENROUTER_API_KEY instead.




---

🛣 Endpoint

POST /api/chat
Content-Type: application/json

{
  "message": "Hello!"
}

✅ Response:

{
  "reply": "Hi! How can I help you today?"
}


---

🔄 Sample Proxy Setup (CORS)

This server is CORS-enabled by default for development.


---

License

MIT
