# 🛸 Synod AI
**Collective Intelligence for shared meeting reporting and summarization**

Synod AI is a high-performance, multi-agent ecosystem designed to transform technical noise into engineering intelligence. By synthesizing live audio, telemetry, and manual notes, we provide UAV teams with a real-time, unified "Source of Truth."

---

## 🏗️ The Ecosystem Architecture

Synod AI uses a **Polyglot Microservices** approach. We leverage **Rust** for mission-critical reliability and **Python** for state-of-the-art agentic intelligence.

### 🛰️ [Synod-Backend](https://github.com/synod-ai/synod-backend)
**The Orchestrator (Rust)**
* Manages high-concurrency **WebSockets** for live room synchronization.
* Handles **RBAC (Level 1-3)** and PostgreSQL data persistence.
* Acts as the secure gateway between the user interface and the AI processing layer.

### 🧠 [Synod-AI-Agent](https://github.com/synod-ai/synod-ai-agent)
**The Brain (Python)**
* Managed by **uv** for high-performance, reproducible AI environments.
* Performs real-time **Whisper-based transcription** and **speaker diarization**.
* Utilizes **recursive RAG** (Retrieval-Augmented Generation) to merge disparate data points into cohesive reports.

### ⚛️ [Synod-Frontend](https://github.com/synod-ai/synod-frontend)
**The Interface (Vite)**
* A real-time, collaborative dashboard built with **React** and **Tailwind CSS**.
* Optimized for **Node.js 22** with native Web-API integration for low-latency audio streaming.

---

## 🛠️ Technology Pillar

| Component | Responsibility | Core Strength |
| :--- | :--- | :--- |
| **Rust** | Auth, Room State, Gateway | Safety & Concurrency |
| **Python** | LLM Synthesis & AI Inference | Flexibility & ML Ecosystem |
| **Docker / K8s** | Microservice Isolation | Scalability |

---

## 🛡️ User Permissions & Workflow

Synod AI is built around a tiered access model to maintain data integrity during sensitive flight operations:

* **Level 3 (Admin):** Full control over meeting rooms, recording status, and final report distribution.
* **Level 2 (Editor):** Capability to draft and **"Push"** notes to the AI, contributing to the live-evolving report.
* **Level 1 (Viewer):** Read-only access to the shared "Truth Feed" and finalized intelligence reports.

---
© 2025 Synod AI Team. All Rights Reserved.
