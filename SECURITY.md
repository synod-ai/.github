# Security Policy

## 1. Our Commitment
The **Synod AI** team takes the security of our robotics ecosystem seriously. Given our application in UAV and autonomous systems, we prioritize data integrity and the prevention of unauthorized system access.

## 2. Supported Versions
We currently provide security updates for the following versions of our microservices:

| Service | Supported Versions |
| :--- | :--- |
| **Synod-Backend (Rust)** | Latest Main |
| **Synod-AI-Agent (Python)** | Latest Main |
| **Synod-Frontend (Vite)** | Latest Main |

## 3. Reporting a Vulnerability
If you discover a security vulnerability, please do not open a public GitHub issue. Instead, follow these steps:

1. **Email us:** Send a detailed report to `erwin.lejeune@tii.ae` (replace with your actual security contact).
2. **Include Details:** Describe the vulnerability, the affected service, and provide a proof-of-concept (PoC) if possible.
3. **Wait for Response:** We acknowledge all valid reports within **48 hours**.

## 4. Scope
We are particularly interested in vulnerabilities related to:
* **RBAC Bypass:** Unauthorized users gaining Level 2 or 3 permissions.
* **Injection Attacks:** Prompt injection in the AI Agent or SQL injection in the Backend.
* **Data Leakage:** Exposure of sensitive UAV telemetry or meeting audio.
* **Denial of Service (DoS):** Attacks that could crash a live flight sync.

## 5. Disclosure Policy
We follow a **90-day responsible disclosure** policy. We ask that you do not share details of the vulnerability publicly until we have had the opportunity to provide a fix for our users.

## 6. Security Architecture Features
* **Memory Safety:** Our core gateway is built in **Rust** to eliminate memory-related vulnerabilities.
* **Dependency Auditing:** We use `uv` and `cargo audit` to scan for known vulnerabilities in our supply chain.
* **Isolation:** All services run in isolated Docker containers to prevent lateral movement.

---
Thank you for helping keep the Synod AI ecosystem secure.
