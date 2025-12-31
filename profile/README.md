# Synod - Collaborative Meeting Platform

> **AI-driven collaborative meeting platform** that provides a "Single Source of Truth" for meeting documentation through multi-user notes, real-time collaboration, and AI-powered assistance.

## 🏗️ Architecture

Synod consists of three main components:

### 📡 [synod-backend](https://github.com/your-org/synod/tree/main/synod-backend)
**Python FastAPI Backend API**
- RESTful API for meetings, notes, users, and labels
- Real-time WebSocket chat (meeting & private messages)
- JWT authentication with Google OAuth2
- PostgreSQL database with async operations
- Background tasks for meeting status updates
- User analytics and year recaps

### 🎨 [synod-frontend](https://github.com/your-org/synod/tree/main/synod-frontend)
**React + TypeScript Frontend**
- Modern responsive UI with dark/light mode
- Markdown editor with live preview
- Calendar view with meeting visualization
- Real-time chat interface
- User profiles with analytics
- Mobile-friendly design

### 🤖 [synod-agent](https://github.com/your-org/synod/tree/main/synod-agent)
**AI Agent Service (Google ADK)**
- AI-powered meeting assistance
- Database tools for meeting management
- Chat API for agent interactions
- Integration with Google AI Studio/Gemini

## 🚀 Quick Start

### Prerequisites
- Docker & Docker Compose (recommended)
- OR Python 3.12+, Node.js 22+, PostgreSQL 14+, Redis
- Google OAuth credentials

### Run Everything with Docker

```bash
# Clone the repository
git clone --recurse-submodules <repository-url>
cd synod

# Set up environment variables
cp synod-backend/.env.example synod-backend/.env
cp synod-agent/.env.example synod-agent/.env
# Edit .env files with your configuration

# Start all services
make up
# OR
docker-compose up
```

**Services will be available at:**
- Frontend: http://localhost:5173
- Backend API: http://localhost:3000
- API Docs: http://localhost:3000/docs
- Agent Service: http://localhost:8000

### Manual Setup

See the [main README](https://github.com/your-org/synod/blob/main/README.md) for detailed setup instructions for each component.

## 📚 Documentation

- **[Main README](https://github.com/your-org/synod/blob/main/README.md)** - Complete setup and development guide
- **[Backend Docs](https://github.com/your-org/synod/tree/main/synod-backend)** - API documentation
- **[Frontend Docs](https://github.com/your-org/synod/tree/main/synod-frontend)** - Frontend development guide
- **[Agent Docs](https://github.com/your-org/synod/tree/main/synod-agent)** - AI Agent service documentation
- **[Docker Guide](https://github.com/your-org/synod/blob/main/DOCKER.md)** - Docker deployment guide

## 🛠️ Technology Stack

- **Backend**: Python 3.12+, FastAPI, PostgreSQL, Redis, WebSockets
- **Frontend**: React 18, TypeScript, Vite, Tailwind CSS, Zustand
- **Agent**: Python 3.12+, FastAPI, Google ADK
- **Infrastructure**: Docker, Docker Compose

## ✨ Key Features

- ✅ OAuth2 Google authentication
- ✅ Real-time meeting chat and private messaging
- ✅ Markdown notes with live preview and drafts
- ✅ Agenda management and meeting reports
- ✅ Calendar view with iCalendar export
- ✅ User analytics and year-by-year recaps
- ✅ Role-Based Access Control (Viewer/Editor/Admin)
- ✅ AI-powered meeting assistance
- ✅ Dark/Light mode theme
- ✅ Mobile-responsive design

## 🤝 Contributing

We welcome contributions! Please see the [main README](https://github.com/your-org/synod/blob/main/README.md) for development setup and contribution guidelines.

## 📝 License

[Add your license here]

---

**Need help?** Check out the [main README](https://github.com/your-org/synod/blob/main/README.md) for detailed documentation and troubleshooting.

