<div align="center">

# Hi 👋, I'm Madhuri H S

### Backend Software Engineer | Java · Python · Spring Boot · Building Scalable Systems

<p>
Building scalable backend systems, REST APIs, and cloud-ready applications.
</p>

<a href="https://github.com/MADHURI-HS"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github"/></a>
<a href="https://www.linkedin.com/in/madhuri-h-s/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin"/></a>
<a href="mailto:hsmadhuri7@gmail.com"><img src="https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=gmail"/></a>
<a href="https://leetcode.com/YOUR_LEETCODE_USERNAME"><img src="https://img.shields.io/badge/LeetCode-FFA116?style=for-the-badge&logo=leetcode"/></a>

</div>

---

### 💫 About Me

Backend Software Engineer with a background in **AI & Machine Learning** (BE, 2026, VTU — CGPA 8.76). I build scalable backend systems with **Java and Spring Boot**, and apply my AI/ML foundation to intelligent, data-driven features when a project calls for it.

- 💼 Data Science Intern @ **Take It Smart (OPC) Pvt Ltd** (Feb–May 2026) — received the **Best Performer** award
- 🎯 Seeking full-time **Software Engineer** roles in Java/Spring Boot backend development — open to GenAI/ML-adjacent roles too
- 📍 Bengaluru, Karnataka — **immediate joiner**
- 🧩 200+ problems solved on LeetCode; currently working through Striver's SDE Sheet
- 🏗️ Comfortable with **Low-Level Design (LLD) and OOP design patterns** — backed by real open-source contributions (see below)

---

### 🛠️ Tech Stack

**Languages:** ![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white) ![Python](https://img.shields.io/badge/Python-3670A0?style=flat-square&logo=python&logoColor=white) ![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=c%2B%2B&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-323330?style=flat-square&logo=javascript&logoColor=F7DF1E)

**Backend:** ![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white) ![Spring WebFlux](https://img.shields.io/badge/Spring%20WebFlux-6DB33F?style=flat-square&logo=spring&logoColor=white) Microservices · RESTful APIs · Spring Data JPA

**System Design:** Low-Level Design (LLD) · OOP Design Patterns (Singleton, Observer, Factory, etc.)

**Frontend:** ![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB) Vite

**Databases & Caching:** ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white) ![MySQL](https://img.shields.io/badge/MySQL-00000F?style=flat-square&logo=mysql&logoColor=white) ![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)

**DevOps & Tools:** ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white) ![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white) ![Postman](https://img.shields.io/badge/Postman-FF6C37?style=flat-square&logo=postman&logoColor=white) AWS (learning)

**AI/ML Tooling:** RAG · LangChain · ChromaDB · OpenAI Embeddings

**Core CS:** Operating Systems · Computer Networks · DBMS · Object-Oriented Programming

---

## 🚀 Featured Projects

### 🔗 URL Shortener
**Production-ready URL shortening service — live and deployed**

A scalable URL shortener converting long URLs into compact Base62-encoded links, with persistent storage, Redis caching, rate limiting, and a Dockerized deployment.

**Tech Stack:** Spring Boot · PostgreSQL · Redis · Bucket4j · Docker · Maven · Render

```text
               Client
                  │
                  ▼
          Spring Boot REST API
                  │
      ┌───────────┴───────────┐
      ▼                       ▼
   Redis Cache          PostgreSQL
      │                       │
      └───────────┬───────────┘
                  ▼
            Response
```

**Highlights:**
- Built REST APIs using **Base62 encoding**, backed by PostgreSQL with JPA
- Reduced repeated database reads with **Redis caching (Upstash)**
- Implemented **API rate limiting with Bucket4j** to prevent abuse
- Configured **Spring Profiles** for clean dev/prod separation
- Full production hardening pass: scrubbed leaked credentials from git history, resolved environment config issues
- Containerized with Docker, deployed live on Render

🔗 **Repo:** https://github.com/MADHURI-HS/url-shortener
<br/>
🌐 **Live Demo:** https://url-shortener-9iuz.onrender.com

---

### ✉️ AI Email Reply Generator
**AI-powered email reply assistant — Chrome Extension + Spring Boot API**

A monorepo containing both frontend and backend, generating contextual, tone-aware email replies directly inside Gmail using Google's Gemini API.

**Tech Stack:** Spring Boot (WebFlux) · React (Vite) · Gemini API · Chrome Extension (Manifest V3) · GitHub Actions CI/CD

```text
React Frontend
       │
       ▼
Spring Boot API (WebFlux)
       │
       ▼
 Gemini API
       │
       ▼
 Generated Reply
```

**Highlights:**
- Non-blocking, async backend built with **Spring WebFlux**
- Chrome Extension injects directly into Gmail's interface
- **CI/CD pipeline with GitHub Actions**, including a custom Dockerfile and test config to handle API-key requirements in CI
- Tone customization: professional, casual, or friendly replies

🔗 **Repo:** https://github.com/MADHURI-HS/email-assistance

---

### 🏋️ Fitness Tracking Microservices Platform *(in progress — repo pushing soon)*
**Microservices-based fitness tracking platform with AI-powered recommendations**

**Tech Stack:** Spring Boot · Spring Cloud · Eureka · API Gateway · RabbitMQ · Keycloak OAuth2 · React · PostgreSQL · Docker

```text
                  Client
                     │
                     ▼
               API Gateway
                     │
             Eureka Discovery
        ┌─────────┼─────────┐
        ▼         ▼         ▼
     User     Activity      AI
    Service    Service   Recommendation
        │
        ▼
 PostgreSQL Database
```

**Highlights:**
- Microservices architecture with **service discovery (Eureka)** and centralized configuration
- **RabbitMQ** for asynchronous, event-driven activity processing
- **Keycloak OAuth2** for secure authentication
- **Gemini API** integration for personalized workout recommendations

---

### 🎓 Smart Attendance System
**AI-powered face recognition attendance system**

**Tech Stack:** Python · OpenCV · YOLOv8 · FaceNet · Streamlit · SQLite

```text
Camera
   │
   ▼
YOLOv8 Detection
   │
   ▼
FaceNet Recognition
   │
   ▼
Duplicate Check
   │
   ▼
SQLite Database
   │
   ▼
Attendance Dashboard
```

**Highlights:**
- Real-time face detection (YOLOv8) and recognition (FaceNet embeddings)
- Interactive **Streamlit** dashboard with live analytics
- Duplicate-entry prevention and CSV export for attendance reports

🔗 **Repo:** https://github.com/MADHURI-HS/smart-attendance-system

---

## 💼 Experience

**Data Science Intern — Take It Smart (OPC) Pvt Ltd** · Feb 2026 – May 2026

- Built machine learning models for predictive analysis
- Performed data preprocessing and feature engineering
- Developed interactive dashboards for data visualization (Python: Pandas, NumPy, Matplotlib)
- Collaborated on AI-based applications and automation tasks
- 🏆 Received the **Best Performer** award

---

## 📜 Certifications

- ☕ **Java + Spring Boot (Basics to Advanced)** — Udemy (Shrayansh Jain)
- ☁️ **AWS Cloud Practitioner** — Coursera (foundational/knowledge-level)
- 📘 **Data Structures & Algorithms** — TakeUforward
- 💡 **Object-Oriented Programming** — TakeUforward
- 🌐 **Computer Networks + Operating Systems** — TakeUforward
- 💻 **Programming in C++** — NPTEL (IIT Kharagpur)

---

## 🌟 Open Source

Contributor to [**java-design-patterns**](https://github.com/iluwatar/java-design-patterns) — merged PRs improving Singleton and Observer pattern implementations and documentation.

---

## 📊 GitHub Stats

<div align="center">

<img src="https://streak-stats.demolab.com?user=MADHURI-HS&theme=github-dark-blue&hide_border=true"/>

<br/>

<img src="https://ghchart.rshah.org/MADHURI-HS" alt="GitHub Contribution Chart"/>

</div>

---

## 📫 Contact Me

📧 **Email:** hsmadhuri7@gmail.com
<br/>
💼 **LinkedIn:** https://www.linkedin.com/in/madhuri-h-s/
<br/>
🐙 **GitHub:** https://github.com/MADHURI-HS

---

<div align="center">

*"Code. Learn. Build. Repeat."* 🚀

</div>
