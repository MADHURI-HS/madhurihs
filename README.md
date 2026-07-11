<div align="center">

# Hi 👋, I'm Madhuri H S

### Backend Software Engineer | Java · Spring Boot · Microservices · Building Scalable Systems

<p>
Building scalable backend systems, REST APIs, and cloud-ready applications.
</p>

<a href="https://github.com/MADHURI-HS"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github"/></a>
<a href="https://www.linkedin.com/in/madhuri-h-s/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin"/></a>
<a href="mailto:madhurihssahani07@gmail.com"><img src="https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=gmail"/></a>
<a href="https://leetcode.com/u/MADHURIHS/"><img src="https://img.shields.io/badge/LeetCode-FFA116?style=for-the-badge&logo=leetcode"/></a>

</div>

---

### About Me

Backend Software Engineer with a BE in **AI & Machine Learning** (2026, VTU — CGPA 8.76). I build scalable backend systems with **Java and Spring Boot** — REST APIs, microservices with service discovery and API gateways, and RAG-based AI applications — backed by a strong academic foundation in AI/ML that I apply hands-on where it's relevant.

- Data Science Intern @ **Take It Smart (OPC) Pvt Ltd** (Feb–May 2026) — received the **Best Performer** award
- Seeking full-time Software Engineer roles — backend and full-stack
- Bengaluru, Karnataka — **immediate joiner**
- 200+ problems solved on LeetCode; currently working through Striver's SDE Sheet
- Comfortable with **Low-Level Design (LLD) and OOP design patterns** — backed by real open-source contributions (see below)

---

### Tech Stack

**Languages:** ![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white) ![Python](https://img.shields.io/badge/Python-3670A0?style=flat-square&logo=python&logoColor=white) ![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=c%2B%2B&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-323330?style=flat-square&logo=javascript&logoColor=F7DF1E)

**Backend:** ![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white) ![Spring Cloud](https://img.shields.io/badge/Spring%20Cloud-6DB33F?style=flat-square&logo=spring&logoColor=white) Microservices · RESTful APIs · Spring Data JPA · OpenFeign · Eureka

**System Design:** Low-Level Design (LLD) · OOP Design Patterns (Singleton, Observer, Factory, etc.)

**Databases & Caching:** ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white) ![MySQL](https://img.shields.io/badge/MySQL-00000F?style=flat-square&logo=mysql&logoColor=white) ![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)

**DevOps & Tools:** ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white) ![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white) ![Postman](https://img.shields.io/badge/Postman-FF6C37?style=flat-square&logo=postman&logoColor=white)

**AI/ML Foundations:** Artificial Intelligence · Machine Learning · Deep Learning · Generative AI · Data Visualization — academic foundation from BE (AI & ML), applied hands-on in projects below

**AI/ML Tooling (Applied):** RAG · Spring AI · Ollama · Qdrant · Vector Embeddings

**Currently Learning:** AWS Cloud Practitioner (in progress)

**Core CS:** Operating Systems · Computer Networks · DBMS · Object-Oriented Programming

---

## Featured Projects

### Spring AI RAG Chatbot
**Locally hosted Retrieval-Augmented Generation chatbot — zero API cost, full local inference**

A context-aware, multi-turn Q&A chatbot grounded in technical documentation, built with Spring AI's ChatClient, running entirely on local infrastructure via Ollama.

**Tech Stack:** Spring Boot · Spring AI · Ollama (nomic-embed-text, llama3.2) · Qdrant · Docker Compose

```text
PDF Document
     │
     ▼
TikaDocumentReader → TextSplitter → Ollama Embeddings → Qdrant
                                                            │
User Question → QuestionAnswerAdvisor ────────────────────┘
     │                    │
MessageChatMemoryAdvisor   Ollama (llama3.2)
     └──────► ChatClient ◄──────┘
                  │
                  ▼
               Answer
```

**Highlights:**
- Built using **Spring AI's ChatClient** with `QuestionAnswerAdvisor` and `MessageChatMemoryAdvisor` for RAG + multi-turn conversation memory
- Document ingestion pipeline: PDF parsing (Apache Tika) → chunking → embedding (Ollama `nomic-embed-text`) → vector storage (Qdrant)
- Diagnosed and fixed a structured-output parsing failure specific to smaller local LLMs
- Fully local inference — no external API costs, no data leaving the machine

**Repo:** https://github.com/MADHURI-HS/spring-ai-rag-chat

---

### School Management Microservices Platform
**Distributed microservices system with service discovery, API gateway, and distributed tracing**

A multi-service Spring Boot application demonstrating core microservices architecture patterns, with verified inter-service communication and request tracing.

**Tech Stack:** Spring Boot · Spring Cloud · Netflix Eureka · Spring Cloud Gateway · OpenFeign · PostgreSQL · Zipkin · Docker

```text
                  Client
                     │
                     ▼
               API Gateway :8222
                     │
          ┌──────────┴──────────┐
          ▼                     ▼
   Student Service :8090  School Service :8070
          │                     │  (OpenFeign call
          ▼                     ▼   via Gateway)
    students DB            schools DB

  Config Server :8888 ── supplies config to all services
  Eureka :8761 ── service discovery/registration
  Zipkin :9411 ── distributed tracing across every request
```

**Highlights:**
- Centralized configuration via **Spring Cloud Config Server**, dynamic service discovery via **Netflix Eureka**
- **API Gateway** routing requests to independently deployable services
- Verified inter-service communication: School service calls Student service via **OpenFeign**, routed through the Gateway
- **Distributed tracing with Zipkin** — full request path and per-hop latency captured for every call
- Diagnosed and resolved a Lombok/JDK 21 compiler incompatibility (`NoSuchFieldError`) across multiple modules

**Repo:** https://github.com/MADHURI-HS/school-management-microservices

---

### URL Shortener
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
- Reduced repeated database reads with **Redis caching (Upstash)**, cutting redirect latency from 40–60ms to 5–10ms
- Implemented **API rate limiting with Bucket4j** to prevent abuse
- Configured **Spring Profiles** for clean dev/prod separation
- Containerized with Docker, deployed live on Render

**Repo:** https://github.com/MADHURI-HS/url-shortener
<br/>
**Live Demo:** https://url-shortener-9iuz.onrender.com

---

### AI Email Reply Generator
**AI-powered email reply assistant — Chrome Extension + Spring Boot API**

A monorepo containing both frontend and backend, generating contextual, tone-aware email replies directly inside Gmail using Google's Gemini API.

**Tech Stack:** Spring Boot (WebFlux) · React (Vite) · Gemini API · Chrome Extension (Manifest V3) · GitHub Actions CI/CD

**Highlights:**
- Non-blocking, async backend built with **Spring WebFlux**
- Chrome Extension injects directly into Gmail's interface
- **CI/CD pipeline with GitHub Actions**, including a custom Dockerfile and test config to handle API-key requirements in CI
- Tone customization: professional, casual, or friendly replies

**Repo:** https://github.com/MADHURI-HS/email-assistance

---

### Smart Attendance System
**AI-powered face recognition attendance system**

**Tech Stack:** Python · OpenCV · Streamlit · MySQL

**Highlights:**
- Real-time face detection and recognition using **OpenCV**
- Interactive **Streamlit** dashboard with attendance history and student records
- Duplicate-entry prevention — attendance marked only once per student per day

**Repo:** https://github.com/MADHURI-HS/smart-attendance-system

---

## Experience

**Data Science Intern — Take It Smart (OPC) Pvt Ltd** · Feb 2026 – May 2026

- Built machine learning models for predictive analysis
- Performed data preprocessing and feature engineering
- Developed interactive dashboards for data visualization (Python: Pandas, NumPy, Matplotlib)
- Collaborated on AI-based applications and automation tasks
- Received the **Best Performer** award

---

## Certifications

- **Java + Spring Boot (Basics to Advanced)** — Udemy (Shrayansh Jain)
- **Data Structures & Algorithms** — TakeUforward
- **Object-Oriented Programming** — TakeUforward
- **Computer Networks + Operating Systems** — TakeUforward
- **Programming in C++** — NPTEL (IIT Kharagpur)

---

## Open Source

Contributor to [**java-design-patterns**](https://github.com/iluwatar/java-design-patterns) — merged PRs improving Singleton and Observer pattern implementations and documentation.

---

## GitHub Stats

<div align="center">

<img src="https://streak-stats.demolab.com?user=MADHURI-HS&theme=github-dark-blue&hide_border=true"/>

<br/>

<img src="https://ghchart.rshah.org/MADHURI-HS" alt="GitHub Contribution Chart"/>

</div>

---

## 📫 Contact Me

- 📧 **Email:** madhurihssahani07@gmail.com
- 💼 **LinkedIn:** https://www.linkedin.com/in/madhuri-h-s/
- 💻 **GitHub:** https://github.com/MADHURI-HS

---

<div align="center">

*"Code. Learn. Build. Repeat."*

</div>
