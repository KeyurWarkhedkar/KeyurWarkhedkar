# Hi, I'm Keyur 👋

Backend developer focused on **distributed systems, event-driven architecture, and production-grade APIs**. I build systems that handle concurrency, failure recovery, and scale — with a strong foundation in Spring Boot, AWS, and database internals. 330+ LeetCode problems. CGPA 9.79.

---

# 🛠 Technical Skills

##### 🌱 Spring Ecosystem
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)
![Spring MVC](https://img.shields.io/badge/Spring_MVC-6DB33F?style=for-the-badge&logo=spring&logoColor=white)
![Spring Data JPA](https://img.shields.io/badge/Spring_Data_JPA-6DB33F?style=for-the-badge&logo=spring&logoColor=white)
![Spring Security](https://img.shields.io/badge/Spring_Security-6DB33F?style=for-the-badge&logo=springsecurity&logoColor=white)
![OAuth2](https://img.shields.io/badge/OAuth2-6DB33F?style=for-the-badge&logo=spring&logoColor=white)
![REST API](https://img.shields.io/badge/REST_API-6DB33F?style=for-the-badge&logo=spring&logoColor=white)

##### ⚙️ Distributed Systems
![Amazon SQS](https://img.shields.io/badge/Amazon_SQS-FF9900?style=for-the-badge&logo=amazonsqs&logoColor=white)
![Event-Driven](https://img.shields.io/badge/Event--Driven_Architecture-FF9900?style=for-the-badge&logo=amazon&logoColor=white)
![Saga Pattern](https://img.shields.io/badge/Saga_Pattern-FF9900?style=for-the-badge&logo=amazon&logoColor=white)
![RabbitMQ](https://img.shields.io/badge/RabbitMQ-FF6600?style=for-the-badge&logo=rabbitmq&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![Firebase FCM](https://img.shields.io/badge/Firebase_FCM-FFCA28?style=for-the-badge&logo=firebase&logoColor=black)

##### 🗄️ Databases
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![Firebase Firestore](https://img.shields.io/badge/Firestore-FFCA28?style=for-the-badge&logo=firebase&logoColor=black)
![Hibernate](https://img.shields.io/badge/Hibernate-59666C?style=for-the-badge&logo=hibernate&logoColor=white)

##### ☁️ Cloud & DevOps
![AWS EC2](https://img.shields.io/badge/AWS_EC2-FF9900?style=for-the-badge&logo=amazonec2&logoColor=white)
![AWS RDS](https://img.shields.io/badge/AWS_RDS-FF9900?style=for-the-badge&logo=amazonrds&logoColor=white)
![AWS ECR](https://img.shields.io/badge/AWS_ECR-FF9900?style=for-the-badge&logo=amazon&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=for-the-badge&logo=grafana&logoColor=white)
![Loki](https://img.shields.io/badge/Loki-F46800?style=for-the-badge&logo=grafana&logoColor=white)
![Cloudflare](https://img.shields.io/badge/Cloudflare-F38020?style=for-the-badge&logo=cloudflare&logoColor=white)

##### 🧪 Testing & Performance
![JUnit5](https://img.shields.io/badge/JUnit5-25A162?style=for-the-badge&logo=junit5&logoColor=white)
![K6](https://img.shields.io/badge/K6-7D64FF?style=for-the-badge&logo=k6&logoColor=white)
![JMeter](https://img.shields.io/badge/JMeter-D22128?style=for-the-badge&logo=apachejmeter&logoColor=white)

##### 🚀 Tools
![Maven](https://img.shields.io/badge/Maven-C71A36?style=for-the-badge&logo=apache-maven&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)

##### 💻 Languages
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=postgresql&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

---

# 🔥 Featured Projects

#### 1. QueueX — Event-Driven Order Processing System ⭐ Flagship

A distributed async order processing system across two Spring Boot microservices — implementing the saga pattern with compensating transactions, transactional outbox, at-least-once delivery via Amazon SQS, and idempotency at every layer. Deployed on AWS with CI/CD and live observability.

⚙️ Technical Highlights:

📬 **Saga Pattern with Compensating Transactions** — inventory reserved, payment attempted with exponential backoff retry; stock automatically restored on payment failure

🔁 **Transactional Outbox Pattern** — events written atomically with business data, published reliably via scheduled poller with retry and dead-letter handling across 7 SQS queues

🔐 **Idempotency at Every Layer** — blind insert + atomic status change guards every consumer against duplicate SQS redeliveries

🚀 **CI/CD Pipeline** — push to main triggers GitHub Actions: Maven build → ECR image push → zero-downtime container redeploy on EC2 via SSH

📊 **Grafana + Loki Observability** — structured JSON logs with MDC-based orderId propagation; full saga trace filterable by order across both services in Grafana Cloud

⚡ **Load Tested** — 46.8 req/s · P95 82ms · 0% error rate under 100 concurrent users (K6)

**Tech Stack:** Spring Boot | Amazon SQS | AWS EC2 | RDS MySQL | ECR | Docker | GitHub Actions | Grafana | Loki | K6

**[View Project →](https://github.com/KeyurWarkhedkar/queue-x)**

---

#### 2. API-Shield — High-Performance API Gateway Middleware

A production-grade API gateway built to protect backend services from abuse, reduce external API costs through intelligent caching, and provide distributed rate limiting with real-time traffic monitoring.

⚙️ Technical Highlights:

⚡ **98.5% API Load Reduction** — prevented ~395 out of 400 external API calls through smart caching

🚦 **Redis-Backed Distributed Rate Limiting** using token bucket algorithm for consistent throttling across instances

📊 **Hot Endpoint Detection** with LRU cache eviction — automatically identifies and caches frequently accessed endpoints

🔥 **15ms Median Latency** for cached responses · 49ms P95 under concurrent load

✅ **JMeter Validated** — 87.5% cache hit ratio across 400 concurrent requests

**Tech Stack:** Spring Boot | Redis | Maven | JMeter

**[View Project →](https://github.com/KeyurWarkhedkar/api-shield)**

---

#### 3. Math Premier League — Concurrent Multi-Team Quiz Platform

A competitive quiz system demonstrating concurrent system design, thread safety, and real-time communication under heavy load — with a focus on diagnosing and fixing race conditions rather than just avoiding them.

⚙️ Technical Highlights:

🧵 **Race condition diagnosed deterministically** using Thread.sleep() with 2 concurrent threads — proved root cause as implicit S lock acquisition during MySQL FK constraint verification

🔒 **Pessimistic locking → atomic SQL update** — 78% throughput improvement and 33% latency reduction while maintaining 0 duplicates and 0 deadlocks

📡 **WebSocket (STOMP) real-time leaderboard** — instant score broadcasting across all connected teams

⚡ **250+ concurrent registrations** with 0 duplicate assignments (K6 validated)

**Tech Stack:** Spring Boot | WebSocket (STOMP) | MySQL | JPA | K6

**[View Project →](https://github.com/KeyurWarkhedkar/Math-Premier-League-Backend)**

---

#### 4. Healio — Smart Appointment & Counselling Platform

Full-stack healthcare counseling platform with event-driven messaging, concurrency-safe booking, and secure OAuth2 authentication.

⚙️ Technical Highlights:

🧠 **Optimistic locking** preventing double-booking during simultaneous slot updates

📬 **RabbitMQ** async notifications — booking confirmations and cancellations without blocking the main flow

🔐 **JWT + Google OAuth2** with Spring Security filter chain

⚡ **Redis** for OTP storage and faster auth flows

**Tech Stack:** Spring Boot | RabbitMQ | MySQL | Redis | Docker | JWT

**[View Project →](https://github.com/KeyurWarkhedkar/healio)**

---

# 💼 Experience

**Backend Developer Intern @ Valsco Technology** *(March 2026 – May 2026)*
- Built a cron-based ETL pipeline to ingest and normalize court case data from multiple government APIs into Firebase Firestore with schema inconsistency handling and failure recovery
- Designed notification system using Firebase Cloud Functions + FCM for real-time Android/iOS case update alerts
- Developed backend workflow replicating National Green Tribunal case search flow — captcha retrieval, query orchestration, structured case extraction

**SDE Intern @ Ealth Technologies** *(January 2026 – February 2026)*
- Eliminated Hibernate N+1 query issue using JOIN FETCH — reduced avg response time from ~180ms → ~100ms
- Applied per-user API rate limiting via token-bucket algorithm; 87% of 100 requests correctly throttled at 5 req/sec (JMeter)
- Moved OTP email sending to async post-commit — reduced failure response time by ~99%
- Deployed Dockerized full-stack app on AWS EC2 with RDS, Redis, and HTTPS via Cloudflare

---

# 📊 Problem Solving

**330+ DSA problems solved** — strong foundation in algorithms, data structures, and optimization

[![LeetCode](https://img.shields.io/badge/LeetCode-000000?style=for-the-badge&logo=leetcode&logoColor=orange)](https://leetcode.com/u/Keyur_Warkhedkar/)

---

# 📊 Language Stats

![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=KeyurWarkhedkar&layout=compact&theme=radical)

---

# 📫 Let's Connect

**Email:** keyurwarkhedkar@gmail.com

**LinkedIn:** [linkedin.com/in/keyurwarkhedkar](https://linkedin.com/in/keyurwarkhedkar)

**GitHub:** [github.com/KeyurWarkhedkar](https://github.com/KeyurWarkhedkar)

**Location:** Pune, India

---

💡 **Open to backend engineering opportunities** | Distributed systems · Spring Boot · AWS
