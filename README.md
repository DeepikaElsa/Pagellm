<div align="center">
  
<img width="full" height="auto" alt="pagelm" src="https://github.com/user-attachments/assets/d3133be1-1931-4132-9301-3596ebb21122" />

# PageLM

**An open source AI powered education platform that transforms study materials into interactive learning experiences, slightly inspired by NotebookLM**


</div>

<p align="center">
  <a href="LICENSE"><img src="https://img.shields.io/badge/License-PageLM%20Community%20License-blueviolet.svg" alt="License: PageLM Community License"></a>
  <a href="https://nodejs.org/"><img src="https://img.shields.io/badge/node-%3E%3D20.0.0-brightgreen.svg" alt="Node.js Version"></a>
  <a href="https://reactjs.org/"><img src="https://img.shields.io/badge/React-18+-blue.svg" alt="React"></a>
  <a href="https://www.typescriptlang.org/"><img src="https://img.shields.io/badge/TypeScript-5.0+-blue.svg" alt="TypeScript"></a>
  <a href="https://discord.gg/P7HaRayqTh"><img alt="Discord" src="https://img.shields.io/discord/1379682804849180844?label=Discord%20server"></a>
</p>

---
</div>

## Demo

<img src=".github/pagelm.png" alt="PageLM Demo"/>

https://github.com/user-attachments/assets/98fae4ef-c2b7-4ad2-bfe9-1e0665eb4d71

<video width="100%" controls>
  <source src=".github/demo.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

> **Note**: If the video doesn't load above, you can [download the demo video directly](.github/demo.mp4)

---

## 🚀 Features

PageLM converts study material into **interactive resources** including quizzes, flashcards, structured notes, and podcasts.  
The platform provides a modern interface for students, educators, and researchers to **enhance learning efficiency** using state-of-the-art LLMs and TTS systems.

### Learning Tools

- **Contextual Chat** – Ask questions about uploaded documents (PDF, DOCX, Markdown, TXT)
- **SmartNotes** – Generate Cornell-style notes automatically from topics or uploaded content
- **Flashcards** – Extract non-overlapping flashcards for spaced repetition
- **Quizzes** – Create interactive quizzes with hints, explanations, and scoring
- **AI Podcast** – Convert notes and topics into engaging audio content for learning on the go
- **Voice Transcribe** - Convert lecture recordings and voice notes into organized, searchable study materials instantly.
- **Homework Planner** - Plans your Homework Smartly using AI, Assists if your stuck.
- **ExamLab** - Simulate any exam, get feedback, and be prepared for the exam
- **Debate** - Debate with AI to improve your Debate skills.
- **Study Companion** - A personalised AI Companion that assists you.

### Supported AI Models

- Google Gemini • OpenAI GPT • Anthropic Claude • xAI Grok • [MiniMax](https://www.minimax.io/) • Ollama (local) • OpenRouter

### Embedding Providers

- OpenAI • Gemini • Ollama

### Technical Highlights

- WebSocket streaming for real-time chat, notes, and podcast generation
- JSON or vector database support for embeddings and retrieval
- File-based persistent storage for generated content
- Markdown-based outputs for structured answers and notes
- Configurable multi-provider setup for LLMs and TTS engines

---

## 🛠️ Technology Stack

| Component      | Technology                               |
| -------------- | ---------------------------------------- |
| **Backend**    | Node.js, TypeScript, LangChain, Langraph |
| **Frontend**   | Vite, React, TailwindCSS                 |
| **Database**   | JSON (default), optional vector DB       |
| **AI/ML**      | Multiple LLM providers, embeddings       |
| **Audio**      | Edge TTS, ElevenLabs, Google TTS         |
| **Deployment** | Docker, Docker Compose                   |
| **Docs**       | pdf-lib, mammoth, pdf-parse              |

---

## ⚡ Getting Started

### Prerequisites

- Node.js v21.18+
- npm or pnpm
- ffmpeg (required for podcast audio)
- Docker (optional)

### Local Development

```bash
# Clone the repository
git clone https://github.com/caviraOSS/pagelm.git
cd pagelm

# Linux:
  chmod 777 ./setup.sh
  ./setup.sh

# Windows:
  Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
  ./setup.ps1

# Manual (Both Linux/Windows):
  # Install dependencies
  cd backend
  npm install
  cd ../frontend
  npm install

  # Setup environment
  cd ..
  npm i -g nodemon
  cp .env.example .env
  # Make sure to configure API keys and settings in .env

  # Run these two commands in separate terminals but inside the project directory.
  # Run backend
  cd backend
  npm run dev

  # Run frontend
  cd frontend
  npm run dev
```

👉 Access at: **http://localhost:5173**

### Docker Deployment

```bash
# Development
docker compose up --build

# Production
docker compose -f docker-compose.yml -f docker-compose.prod.yml up -d --build
```

- Frontend: http://localhost:5173 (dev) / http://localhost:8080 (prod)
- Backend: http://localhost:5000

---

## ⚙️ Configuration

All configuration is handled via environment variables:

- **LLM Provider** – Choose your model backend
- **TTS Engine** – Select speech service for podcasts
- **Database Backend** – JSON or vector DB
- **File Upload Limits** – Customize size/format limits

See `.env.example` for all options.

---


## 📜 License

Licensed under the **CaviraOSS Community License**.  
Free to use, share, and modify for personal and educational purposes.  
Commercial use or resale requires prior written permission from CaviraOSS.

See [LICENSE](LICENSE.md) for full terms.

---

<div align="center">


</div>
