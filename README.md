# Hi, I'm Eugene Shin

<img width="1280" height="720" alt="FullSizeRender 크게" src="https://github.com/user-attachments/assets/7da828cd-8ee5-4a7d-a94e-7ddbbbac5247" />

Backend & AI Developer based in Seoul, South Korea.

Passionate about backend developments, and server systems with a strong interest in AI. 
Always eager to learn new technologies and ready to adapt, contribute, and communicate effectively in any environment.

🔗 [LinkedIn](https://www.linkedin.com/in/Eugene-Shin-Dev) | 🐈‍⬛ [GitHub](https://github.com/Eugene-Shin) | 📝 [Tistory](https://devzin.tistory.com/)

---

## 🎓 Education

**Dongguk University** · Seoul, Korea · Mar 2021 – Feb 2027 (Expected)

Bachelor of Engineering in Computer Science and Engineering

- **GPA:** 4.06 / 4.5
- **Academic Excellence Scholarship:** Spring 2021, Fall 2021, Spring 2022, Fall 2022, Fall 2025, Spring 2026

---

## 📂 Projects

### 🚆 Seoul Metro Corporation Complaint Dispatcher
<img width="1280" height="960" alt="IMG_7207 크게" src="https://github.com/user-attachments/assets/a32510f2-0a27-418a-8e1d-884cf2f28531" />

**Backend & ML Developer** | *Mar. 2026 – Present* <br>
*Automated Complaint Classification & Department Dispatch System*

- **Distributed Processing:** Implemented asynchronous inter-service communication using Apache Kafka across three topics — embedding trigger, batch file classification request, and single-complaint classification request — with callback-based result propagation.
- **AI Pipeline:** Applied a two-stage RAG pipeline — KURE-v1 embeddings + pgvector cosine similarity for process code assignment, then top-N retrieval + Qwen3.6 27B for department dispatching.
- **Multi-Environment Configuration:** Separated deployment configs across two environments — on-premises (Docker Compose) and AWS ECS — using Spring profile-based YAML files, environment-specific Dockerfiles, and per-environment Nginx configurations.
- **LLM Integration:** Self-hosted Qwen3.6 27B on a dedicated server using Ollama and integrated it via the OpenAI-compatible REST API, enabling seamless replacement without SDK changes.
- **CI/CD:** Automated the full deployment pipeline with GitHub Actions — on push to main, builds a Gradle JAR, packages three Docker images (Spring Boot, FastAPI, Nginx), pushes them to AWS ECR with commit SHA tags, and force-deploys each service to AWS ECS by registering updated task definitions with injected GitHub Secrets.

### 🌤️ Bid Weather
<img width="1243" height="659" alt="스크린샷 2026-05-29 오후 5 52 19" src="https://github.com/user-attachments/assets/a17f8207-f102-425b-add2-4e9cbadb0ec0" />

**Backend & ML Developer** | *Mar. 2026 – June. 2026* <br>
*Procurement Demand Forecasting Service Based on Weather Data*

- **Modeling:** Trained two LightGBM regression models to predict the number of public procurement announcements based on weather, date, and auto regressive-lag features.
- **Async Event Pipeline:** Designed a Kafka-based async pipeline — Spring Boot scheduler triggers daily data ingestion (G2B, KMA, Holiday APIs), publishes events to Kafka, and the ai-server consumes them to run classification and forecasting sequentially.
- **Backend System:** Built REST APIs with Spring Boot and FastAPI; real-time prediction results delivered to the frontend via Server-Sent Events (SSE). PostgreSQL with pgvector for vector similarity search, Flyway for schema migration, Nginx as reverse proxy.
- **Deployment:** Containerized the entire backend service with Docker Compose and visualized results through a dashboard interface.

### 🛡️ Fargate Smishing Analyzer

**Backend Developer** | *Jan. 2026 - Feb. 2026* <br>
*Remote Smishing Link Execution & AI-Based Threat Analysis Service*

- **Containerized Execution:** Built and optimized Docker images to safely execute suspicious links in isolated remote environments.
- **Threat Scoring:** Designed a malicious scoring system to quantify risk levels based on execution results and heuristics.
- **Cloud Architecture:** Leveraged AWS Fargate to dynamically spawn analysis containers, isolating potentially harmful workloads from the main system.
- **AI Explanation:** Integrated AI-based analysis to provide interpretable summaries of detected threats.

### 🗺️ Location-Based Discount Recommender

**Backend Developer (ETL & Data Pipeline)** | Sep. 2025 - Dec. 2025 <br>
*Conversational Mobile App for Location-Based Discount Recommendations*

- **Data Pipeline:** Designed and implemented an ETL pipeline to collect and normalize promotional data from financial institutions and partner services.
- **Web Crawling:** Built a scheduled crawling system using Playwright, automating data extraction and ingestion into the database.
- **AI Integration:** Supported RAG (Retrieval-Augmented Generation) architecture by managing vector embeddings and data preprocessing for recommendation quality.
- **Data Reliability:** Ensured data freshness and consistency through periodic batch processing and validation logic.

---

## 🏆 Awards & Activities
<img width="1280" height="960" alt="IMG_6898 크게" src="https://github.com/user-attachments/assets/bf941909-b51d-443b-9cfa-19e78e036870" />

- **Dongguk University Computer Engineering Student Council** - Administrative Staff | *2021*
- **Dongguk University Computer Engineering Student Council** - Head of Administration | *2022*
- **GDG (Google Developer Groups)** - Study Participant | *Winter 2025*
- **ORACLE** - Seminar Participant | *Mar. 2026*
- **UMC (University MakeUs Challenge)** - Challenger (10th) & Server Part | *Mar. 2026 – Present*

---

## 🛠️ Technical Skills

<h4> Languages </h4>
<div align="left">
  <img src="https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white" />&nbsp
  <img src="https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54" />&nbsp
</div>

<h4> Frameworks & Libraries </h4>
<div align="left">
  <img src="https://img.shields.io/badge/springboot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white" />&nbsp
  <img src="https://img.shields.io/badge/FastAPI-005571?style=for-the-badge&logo=fastapi" />&nbsp
</div>

<h4> Database </h4>
<div align="left">
  <img src="https://img.shields.io/badge/mysql-4479A1.svg?style=for-the-badge&logo=mysql&logoColor=white" />&nbsp
  <img src="https://img.shields.io/badge/postgresql-4169E1.svg?style=for-the-badge&logo=postgresql&logoColor=white" />&nbsp
</div>

<h4> Infra & DevOps </h4>
<div align="left">
  <img src="https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white" />&nbsp
  <img src="https://img.shields.io/badge/Amazon%20EC2-FF9900?style=for-the-badge&logo=amazonEC2&logoColor=white" />&nbsp
  <img src="https://img.shields.io/badge/nginx-%23009639.svg?style=for-the-badge&logo=nginx&logoColor=white" />&nbsp
  <img src="https://img.shields.io/badge/Apache%20Kafka-000?style=for-the-badge&logo=apachekafka&logoColor=white" />&nbsp
  <img src="https://img.shields.io/badge/github%20actions-%232671E5.svg?style=for-the-badge&logo=githubactions&logoColor=white" />&nbsp
  <img src="https://img.shields.io/badge/AWS-%23FF9900.svg?style=for-the-badge&logo=amazon-aws&logoColor=white" />&nbsp
</div>

---

## 📫 Contact

- 📧 tdw0312@gmail.com
- 📱 +82 10 8767 4204
