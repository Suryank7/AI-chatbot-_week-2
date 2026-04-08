# AI Chatbot Frontend

A modern, responsive AI chatbot interface built using React.js, designed with a clean UI and smooth user experience inspired by ChatGPT and other SaaS products.

## Overview

This project focuses on building a scalable and production-ready chatbot frontend that interacts with an AI API to generate responses. It demonstrates strong frontend skills, UI/UX design, and API integration.

## Features

* **Real-time chat interface**
* **AI-powered responses** (via API integration)
* **Clean and modern UI design**
* **Dark / Light mode support**
* **Typing indicator animation**
* **Chat history** (stored locally)
* **Auto-scroll to latest message**
* **Responsive design** (mobile + desktop)
* **Copy message functionality**
* **Clear chat option**

## Tech Stack

* **Frontend:** React.js (Hooks & Functional Components)
* **State Management:** Context API
* **Styling:** Tailwind CSS
* **API Calls:** Fetch / Axios
* **Animations:** Framer Motion (optional)

## Project Structure

```text
src/
│── components/
│   ├── Sidebar.jsx
│   ├── ChatWindow.jsx
│   ├── MessageBubble.jsx
│   ├── InputBox.jsx
│   └── Loader.jsx
│
│── context/
│   └── ChatContext.jsx
│
│── services/
│   └── api.js
│
│── hooks/
│   └── useChat.js
│
│── App.jsx
│── main.jsx
Installation & Setup
1. Clone the repository

Bash
git clone [https://github.com/your-username/ai-chatbot-frontend.git](https://github.com/your-username/ai-chatbot-frontend.git)
cd ai-chatbot-frontend
2. Install dependencies

Bash
npm install
3. Setup environment variables
Create a .env file in the root directory:

Code snippet
VITE_OPENAI_API_KEY=your_api_key_here
4. Run the project

Bash
npm run dev
API Integration
The chatbot connects to an AI API (such as OpenAI) to generate responses.

Example request structure:

JavaScript
export const sendMessage = async (message) => {
  const response = await fetch("API_ENDPOINT", {
    method: "POST",
    headers: {
      "Content-Type": "application/json",
    },
    body: JSON.stringify({ message }),
  });
  return response.json();
};
Deployment
You can easily deploy this project using:

Vercel

Netlify

Build command:

Bash
npm run build
Future Improvements
Voice input & output

Authentication system

Backend integration (MongoDB / Firebase)

Multi-chat support

Markdown & code highlighting enhancements

Contributions
This is a personal project created for learning and portfolio purposes. External contributions are not accepted.

License
This project is licensed under the MIT License.

Author
Suryank B.Tech Student | Developer