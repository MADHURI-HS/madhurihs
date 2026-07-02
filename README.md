<h1 align="center">Hi 👋, I'm Madhuri H S</h1>
<h3 align="center">Backend Software Engineer | Java · Python · Spring Boot · Building Scalable Systems</h3>

<p align="center">
  <a href="https://www.linkedin.com/in/madhuri-h-s/" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white" />
  </a>
  <a href="mailto:hsmadhuri7@gmail.com">
    <img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white" />
  </a>
  <a href="https://github.com/MADHURI-HS" target="_blank">
    <img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" />
  </a>
</p>

---

### 💫 About Me

- 🎓 BE in **AI & Machine Learning** (2026), Vijaya Vittala Institute of Technology, VTU — **CGPA 8.76**
- 💼 Data Science Intern @ **Take It Smart (OPC) Pvt Ltd** (Feb–May 2026) — received the **Best Performer** award
- 🎯 Seeking full-time **Software Engineer** roles in **Java / Spring Boot backend development**, with openness to GenAI/ML-adjacent positions
- 📍 Based in Bengaluru, Karnataka — **immediate joiner**
- 🧩 Solved 200+ problems on LeetCode; currently working through Striver's SDE Sheet
- 🌱 Continuously building — from REST APIs to microservices to applied GenAI (RAG pipelines)

---

### 🛠️ Skills & Tech Stack

**Languages:** ![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white) ![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=c%2B%2B&logoColor=white) ![Python](https://img.shields.io/badge/Python-3670A0?style=flat-square&logo=python&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-323330?style=flat-square&logo=javascript&logoColor=F7DF1E)

**Backend:** ![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white) ![Spring WebFlux](https://img.shields.io/badge/Spring%20WebFlux-6DB33F?style=flat-square&logo=spring&logoColor=white) Microservices · RESTful APIs

**System Design:** Low-Level Design (LLD) · OOP Design Patterns (Singleton, Observer, Factory, etc.)

**Frontend:** ![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB) Vite

**Databases & Caching:** ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white) ![MySQL](https://img.shields.io/badge/MySQL-00000F?style=flat-square&logo=mysql&logoColor=white) ![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)

**DevOps & Tools:** ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white) ![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white) ![Postman](https://img.shields.io/badge/Postman-FF6C37?style=flat-square&logo=postman&logoColor=white)

**AI/ML Tooling:** RAG · LangChain · ChromaDB · OpenAI Embeddings

**Core CS Subjects:** Operating Systems · Computer Networks · DBMS · Object-Oriented Programming

---

### 🚀 Featured Projects

#### 🔗 [URL Shortener](https://github.com/MADHURI-HS/url-shortener) — [Live Demo](https://url-shortener-9iuz.onrender.com)
A production-hardened URL shortening service built and deployed end-to-end, from Base62 encoding logic to rate-limited public deployment.

**Tech Stack:** ![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white) ![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

- Built REST APIs for URL shortening using **Base62 encoding**, backed by **PostgreSQL** with JPA
- Implemented **Redis caching (Upstash)** to reduce database reads on high-frequency lookups
- Added **API rate limiting with Bucket4j** to protect against abuse
- Configured **Spring Profiles** for clean dev/prod environment separation
- Containerized with **Docker** and deployed live on **Render**
- Performed a full production hardening pass: scrubbed leaked credentials from git history, resolved environment-specific config issues

---

#### ✉️ [AI Email Writer](https://github.com/MADHURI-HS/email-assistance)
A Chrome extension paired with a Spring Boot API that generates contextual, tone-aware email replies directly inside Gmail.

**Tech Stack:** ![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white) ![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB) ![JavaScript](https://img.shields.io/badge/JavaScript-323330?style=flat-square&logo=javascript&logoColor=F7DF1E) ![GitHub Actions](https://img.shields.io/badge/CI%2FCD-2088FF?style=flat-square&logo=githubactions&logoColor=white)

- Built a **Spring WebFlux**-based backend for non-blocking, async API calls to the Gemini API
- Developed a **React (Vite)** frontend and a Chrome Extension (Manifest V3) that injects directly into Gmail
- Set up a **CI/CD pipeline with GitHub Actions**, including a custom Dockerfile and test configuration to handle API-key requirements in CI
- Supports tone customization (professional, casual, friendly) for generated replies

---

#### 🏋️ Fitness Tracking Microservices Platform *(repo pushing soon)*
A full-stack fitness tracking platform built on a microservices architecture with event-driven communication and AI-powered recommendations.

**Tech Stack:** ![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white) ![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB) ![RabbitMQ](https://img.shields.io/badge/RabbitMQ-FF6600?style=flat-square&logo=rabbitmq&logoColor=white)

- Designed a microservices architecture with **service discovery (Eureka)** and centralized configuration
- Used **RabbitMQ** for asynchronous, event-driven activity processing
- Integrated **Keycloak OAuth2** for secure authentication
- Connected the **Gemini API** to generate personalized workout recommendations
- Built the frontend with **React** and Redux Toolkit

---

#### 📸 [Smart Attendance System with Face Recognition](https://github.com/MADHURI-HS/smart-attendance-system)
A computer-vision-based attendance system with real-time face detection and an interactive analytics dashboard.

**Tech Stack:** ![Python](https://img.shields.io/badge/Python-3670A0?style=flat-square&logo=python&logoColor=white) ![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white) ![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

- Implemented real-time face detection and recognition using **OpenCV**
- Built an interactive **Streamlit** dashboard with live camera feed and attendance analytics
- Added duplicate-entry prevention logic and CSV export for attendance reports
- Persisted data in **MySQL**, containerized with **Docker**

---

#### 🤖 DevFolio AI — RAG-based Chatbot (Multi-Module Microservices)
An applied GenAI project: a Retrieval-Augmented Generation chatbot built as a multi-module Maven microservices system.

**Tech Stack:** ![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white) ![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)

- Structured as separate `ingestion-service`, `rag-service`, and `api-gateway` modules
- Used **pgvector** for vector storage and **OpenAI embeddings** for semantic search
- Built on **Spring Boot 3.2.5** with a clean service-separation architecture

---

### 📜 Certifications

- **Java + Spring Boot (Basics to Advanced)** — Udemy (Shrayansh Jain)
- **AWS Cloud Practitioner** — Coursera (foundational/knowledge-level)
- **NPTEL C++** — IIT Kharagpur
- **Computer Networks + Operating Systems** — TakeUforward

---

### 🌟 Open Source

- Contributor to [**java-design-patterns**](https://github.com/iluwatar/java-design-patterns) — merged PRs improving Singleton and Observer pattern implementations and documentation

---

### 📊 GitHub Stats

<div align="center">

![GitHub Streak](https://github-readme-streak-stats.herokuapp.com/?user=MADHURI-HS&theme=radical)

</div>

---

<p align="center"><i>"Code. Learn. Repeat."</i> 🚀</p>
