# Contributing to Synod AI

Thank you for your interest in contributing to Synod AI! We prioritize **safety, performance, and reproducible AI**.

## 🏗️ Multi-Repo Workflow

Synod AI is split into specialized repositories. Please ensure you are opening your Pull Request (PR) in the correct location:
- **`synod-backend`**: Core logic, API, and safety-critical code (Rust).
- **`synod-ai-agent`**: AI models, synthesis logic, and data processing (Python/uv).
- **`synod-frontend`**: User interface and real-time visualization (Vite/Node).

---

## 🛠️ Development Standards

### 🦀 Rust (Backend)
- **Formatting:** Always run `cargo fmt` before committing.
- **Safety:** Avoid `unwrap()` in production code. Use proper error handling with `Result`.
- **Testing:** New features must include unit tests.

### 🐍 Python (AI Agent)
- **Environment:** We use **uv** for all dependency management. Do not check in `pip` requirements.txt files.
- **Typing:** Use Python type hints (`mypy` compatible) for all function signatures.
- **Documentation:** Use Docstrings to explain complex AI prompt logic or telemetry processing.

### ⚛️ Frontend
- **Linting:** Ensure `eslint` passes.
- **Performance:** Avoid unnecessary re-renders in the real-time "Truth Feed."

---

## 🔄 Pull Request Process

1. **Fork & Branch:** Create a feature branch (e.g., `feat/uav-telemetry-sync`).
2. **Local Validation:** Ensure all tests pass in the specific repo.
3. **Integration Test:** If your change affects the API contract, verify it against the `synod-deploy` docker-compose setup.
4. **Documentation:** Update relevant READMEs or inline comments if your changes impact the architectural flow.
5. **Review:** All PRs require at least one approval from the maintainer team.

---

## 🛡️ Coding Philosophy
* **Performance first:** If a task can be done in Rust, do it there.
* **Context is King:** The AI Agent should always be provided with the most accurate metadata (timestamps, speaker IDs).
* **Fail Gracefully:** In a UAV environment, a service crash can be critical. Ensure robust retry logic and error logging.

---
Thank you for helping us build optimal shared communication!
