# NeuroInkX Website Chatbot

This project adds a **hybrid chatbot** to the company website built with
**React + Vite (frontend)** and **MERN (backend)**.\
The chatbot provides **instant FAQ responses** from a MongoDB knowledge
base and falls back to **AI API (e.g., OpenAI, Dialogflow)** for more
complex queries.

------------------------------------------------------------------------

## 🚀 Features

-   💬 Chat bubble + popup widget in React (frontend).
-   ⚡ Instant responses for FAQs (MongoDB search).
-   🤖 AI fallback for unknown queries (OpenAI/Dialogflow).
-   🗂 Chat history storage in MongoDB.
-   📱 Responsive design for desktop & mobile.

------------------------------------------------------------------------

## 🛠️ Tech Stack

-   **Frontend:** React + Vite
-   **Backend:** Node.js + Express
-   **Database:** MongoDB
-   **AI Layer:** OpenAI API (default) / Dialogflow / Rasa (optional)
-   **Hosting:** AWS (EC2/Lambda + S3/CloudFront)

------------------------------------------------------------------------

## 📂 Project Structure

    /frontend       → React + Vite chatbot widget
    /backend        → Express APIs (chat, history, webhook)
    /db             → MongoDB (FAQ + chat logs)
    /ai             → AI integration (OpenAI/Dialogflow)

------------------------------------------------------------------------

## ⚡ Getting Started

### 1. Clone the repo

``` bash
git clone https://github.com/your-org/chatbot-project.git
cd chatbot-project
```

### 2. Install dependencies

``` bash
# frontend
cd frontend
npm install

# backend
cd ../backend
npm install
```

### 3. Set up environment variables

Create a `.env` file in `/backend` with:

    MONGO_URI=your_mongodb_connection
    AI_PROVIDER=openai
    OPENAI_API_KEY=your_openai_key
    PORT=5000

### 4. Run locally

``` bash
# Start backend
cd backend
npm run dev

# Start frontend
cd ../frontend
npm run dev
```

Frontend will run on `http://localhost:5173`\
Backend will run on `http://localhost:5000`

------------------------------------------------------------------------

## 🧪 Testing

-   Run frontend and backend locally.
-   Open chatbot on website → ask an FAQ → check instant response.
-   Try unknown query → AI fallback should reply.
-   Verify chat history saved in MongoDB.

------------------------------------------------------------------------

## 📌 Roadmap
-   [ ] Train custom AI model with company data
-   [ ] Add analytics dashboard for chat logs
-   [ ] Integrate voice-based chat
