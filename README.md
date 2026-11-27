# Hi, I'm Pamaljith Ranasinghe 👋

**Software Engineer** based in Colombo, Sri Lanka. I build full-stack systems and AI platforms where coding agents work alongside people.

[![Portfolio](https://img.shields.io/badge/Portfolio-pamaljithranasinghe.dev-0A66C2?style=flat)](https://pamaljithranasinghe.dev)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-pamal--ranasinghe-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/pamal-ranasinghe)
[![Email](https://img.shields.io/badge/Email-pamalranasinghe464%40gmail.com-D14836?style=flat&logo=gmail&logoColor=white)](mailto:pamalranasinghe464@gmail.com)

---

## About me

- 5+ years building full-stack systems, from backend architecture and APIs to cloud deployments.
- Owned the backend of a multi-tenant learning platform serving **20+ tenants**, shipped **12-15 features** end to end on schedule, and cut slow API responses from **~3-4 s to ~300 ms**.
- Now working on **agentic engineering**: MCP servers, agent skills, and governed AI workflows with evaluation and human approvals.
- Mentor junior developers through code reviews and design guidance.
- Currently pursuing an **MSc in Artificial Intelligence** at the University of Moratuwa.

---

## Tech stack

| Area | Tools |
| --- | --- |
| **Languages** | PHP, Python, Java, JavaScript, TypeScript, HTML, CSS, SQL |
| **Backend & APIs** | Laravel (Queues, Scheduler, Managers), FastAPI, Flask, REST, GraphQL, JWT, Rate Limiting, Idempotent APIs, Multi-Tenancy |
| **Frontend** | React, TypeScript, Tailwind CSS, Vite, JavaFX, jQuery |
| **Databases** | MySQL, PostgreSQL, MongoDB, Redis, SQLite |
| **Cloud & DevOps** | AWS (EC2, S3, Lambda, API Gateway, RDS, ElastiCache, SES, IAM, CloudWatch, Bedrock), Docker, nginx, CI/CD, Linux, Git |
| **AI & Agentic Engineering** | MCP Servers, AI Agent Skills, Claude Code, Tool/Function Calling, Agentic Workflow Design, LLM Integration, Prompt Engineering, AI Evaluation & Governance |
| **Integrations** | PayHere, Commercial Bank, Stripe, Google Pay, Bulk SMS & Email, Receipt Printers & Cash Drawers |
| **Practices** | System Design, Concurrency, Offline-First Sync, OOP, SOLID, Design Patterns, Agile/Scrum, Code Reviews |

---

## Featured projects

### 🎓 ClassHub: Social Learning Platform for Tuition Classes *(in development)*

A platform for tuition classes in Sri Lanka.

**Stack:** Laravel (PHP 8.3), MySQL, Redis, AWS S3, React 19, TypeScript, Tailwind CSS, Vite, Docker, nginx

- **Architecture:** layered backend (controllers, services, repositories) that separates request handling, business rules and database access.
- **Patterns:** request validation classes, a standard result object for service responses, and a Manager pattern for swappable SMS gateways (Text.lk).
- **Security:** JWT authentication with token refresh, and rate limits on login, registration and read/write traffic.
- **Reliability:** idempotent writes (a unique request key, a lock, and a 24-hour saved-response cache per user and route) and request-ID tracing linked to structured error logs.
- **Async & caching:** Redis caching and locks; queued jobs with retries, timeouts and failure handling; scheduler and queues for bulk SMS and email campaigns.
- **Payments:** PayHere integration with subscription and pay-as-you-go billing models.

### 🧾 BillBook: Windows POS & Inventory System *(v1.3.9)*

A desktop point-of-sale system that keeps working when the internet drops.

**Stack:** Java, JavaFX, SQLite, PostgreSQL, JDBC, Maven, ESC/POS thermal printing

- **Concurrency:** the UI thread stays free while background worker threads handle slow work and hand results back to the screen safely.
- **Thread safety:** a single-thread print queue prints receipts in order without blocking the cashier; a lock lets one transaction at a time use the shared database connection.
- **Receipt printing:** receipts sized for 58/80 mm paper rolls, background printer warm-up, and Code 128 / EAN-13 barcode generation.
- **Cash drawer:** drawer-open signals sent directly to the printer, with a shared print lock so they never corrupt a receipt.
- **Offline detection:** a watcher thread checks the hosted PostgreSQL every 3-5 s and shows whether the system is local, online or offline.
- **Offline sync:** offline bills queue in a local SQLite store and upload in order with their original time and cashier; failed bills are kept with the reason for retry; offline sign-in uses salted password hashes valid for 30 days.
- **Integrity:** all-or-nothing transactions with rollback, audit entries written in the same transaction, role-based access, background backups written atomically, and in-place schema migrations.
- **Delivery:** Maven build and Windows installer, in-app updates from GitHub Releases verified by SHA-256, and Sinhala/Tamil item names with built-in transliteration.

### 🤖 Spine: Governed AI Engineering Platform *(work project, Limark Technologies)*

- Expert-labelled golden sets act as both specification and CI/CD regression gate, with auditable human approvals and shared guardrails and evaluation.
- Built the Spine MCP server (Python FastMCP) and reusable agent skills, so AI coding agents such as Claude Code can retrieve approved golden sets and apply them while building and reviewing code.
- Services built with FastAPI and MongoDB on AWS (Lambda, S3, Bedrock), plus a React portal.

---

## Experience

| Role | Company | Period |
| --- | --- | --- |
| Software Engineer (Full-Stack) | Limark Technologies | May 2026 - Present |
| Software Engineer (Full-Stack) | Creative Software (Creative E-Learning) | May 2024 - Apr 2026 |
| Associate Software Engineer | Wijeya Newspapers Ltd | Nov 2022 - Apr 2024 |
| Trainee Software Engineer | Global Edulink | Mar 2022 - Oct 2022 |
| Trainee Software Engineer | Binary Technologies International | Jun 2021 - Dec 2021 |

---

## Education and publication

- **MSc in Artificial Intelligence**, University of Moratuwa (2026 - Present)
- **BSc (Hons) in Information Technology, Software Engineering**, SLIIT (2023)
- 📄 [E-Learning Assistive System for Deaf and Mute Students](https://ieeexplore.ieee.org/document/10025212) (IEEE)

---

## Let's connect

- 🌐 Portfolio: [pamaljithranasinghe.dev](https://pamaljithranasinghe.dev)
- 💼 LinkedIn: [pamal-ranasinghe](https://www.linkedin.com/in/pamal-ranasinghe)
- 📧 Email: [pamalranasinghe464@gmail.com](mailto:pamalranasinghe464@gmail.com)

I'm open to software engineering opportunities, especially roles that combine backend engineering with AI and agentic systems.
