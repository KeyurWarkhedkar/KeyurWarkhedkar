# Hi, I'm Keyur 👋

I'm a backend developer who loves turning ideas into reliable and scalable services. I work primarily with **Spring Boot, JPA, Security, Docker, and Redis.** With strong problem-solving skills backed by 300+ LeetCode solutions, I constantly push myself to design smart and efficient backend workflows that improve user experience and system performance.

# 🛠 Technical Skills

##### 🌱 **Spring Ecosystem**
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)
![Spring MVC](https://img.shields.io/badge/Spring_MVC-6DB33F?style=for-the-badge&logo=spring&logoColor=white)
![Spring Data JPA](https://img.shields.io/badge/Spring_Data_JPA-6DB33F?style=for-the-badge&logo=spring&logoColor=white)
![Spring Security](https://img.shields.io/badge/Spring_Security-6DB33F?style=for-the-badge&logo=springsecurity&logoColor=white)
![Spring](https://img.shields.io/badge/Spring-6DB33F?style=for-the-badge&logo=spring&logoColor=white)
![REST API](https://img.shields.io/badge/REST_API-6DB33F?style=for-the-badge&logo=spring&logoColor=white)
![JPA](https://img.shields.io/badge/JPA-6DB33F?style=for-the-badge&logo=spring&logoColor=white)
![JDBC](https://img.shields.io/badge/JDBC-6DB33F?style=for-the-badge&logo=spring&logoColor=white)
![OAuth2](https://img.shields.io/badge/OAuth2-6DB33F?style=for-the-badge&logo=spring&logoColor=white)

##### 🗄️ **Databases And ORMs**
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![Hibernate](https://img.shields.io/badge/Hibernate-59666C?style=for-the-badge&logo=hibernate&logoColor=white)

##### 🔧 **DevOps**
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
[![Render](https://img.shields.io/badge/Render-46F3B7?style=for-the-badge&logo=render&logoColor=white)](https://render.com)
[![Railway](https://img.shields.io/badge/Railway-0B0D0E?style=for-the-badge&logo=railway&logoColor=white)](https://railway.app)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)

##### 🔄 **Message Brokers & Caching**
![RabbitMQ](https://img.shields.io/badge/RabbitMQ-FF6600?style=for-the-badge&logo=rabbitmq&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)

##### 🧪 **Testing & Performance**
![JUnit5](https://img.shields.io/badge/JUnit5-25A162?style=for-the-badge&logo=junit5&logoColor=white)
![Mockito](https://img.shields.io/badge/Mockito-25A162?style=for-the-badge)
![K6](https://img.shields.io/badge/K6-7D64FF?style=for-the-badge&logo=k6&logoColor=white)

##### 🔐 **Security & Authentication**
![JWT](https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white)
![OAuth2](https://img.shields.io/badge/OAuth2-6DB33F?style=for-the-badge&logo=spring&logoColor=white)

##### 🚀 **Tools**
![Maven](https://img.shields.io/badge/Maven-C71A36?style=for-the-badge&logo=apache-maven&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)
![Swagger](https://img.shields.io/badge/Swagger-85EA2D?style=for-the-badge&logo=swagger&logoColor=black)

##### 💻 *Languages*
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=postgresql&logoColor=white)

---

# 🔥 Featured Projects

#### 1. API-Shield — High-Performance API Gateway Middleware
A production-grade API gateway built to protect backend services from abuse, reduce external API costs through intelligent caching, and provide distributed rate limiting with real-time traffic monitoring.

⚙️ Technical Highlights:

⚡ 98.5% API Load Reduction — Prevented ~395 out of 400 external API calls through smart caching strategies

🚦 Redis-Backed Distributed Rate Limiting using Token Bucket Algorithm for consistent throttling across instances

📊 Hot Endpoint Detection with LRU Cache Eviction — Automatically identifies and caches frequently accessed endpoints

🔥 15ms Median Latency for cached responses with 49ms P95 under concurrent load

📈 Real-Time Metrics Endpoint exposing cache hit ratios, forwarded requests, and throttled traffic

🧩 Filter Chain Architecture enabling modular traffic monitoring, caching, and rate limiting layers

✅ JMeter Validated Performance — 87.5% cache hit ratio across 400 concurrent requests with zero inconsistencies

**Tech Stack:** Spring Boot | Redis | Maven | JMeter

**[View Project →](https://github.com/KeyurWarkhedkar/api-shield)**

---

#### 2. Math Premier League Portal
A competitive quiz system demonstrating concurrent system design, thread safety, and real-time communication patterns under heavy load conditions.

⚙️ Technical Highlights:

🧵 Thread-Safe Question Assignment handling 280+ concurrent requests without conflicts

🧩 Zero Duplicate Assignments under load — validated through K6 performance testing

🔒 Pessimistic Locking & Database Constraints ensuring race-condition prevention during quiz sessions

📡 WebSocket-Based Real-Time Leaderboard for instant score broadcasting across connected teams

⚡ Sub-120ms P95 Response Time under peak concurrency load

**Tech Stack:** Spring Boot | WebSocket (STOMP) | MySQL | JPA | K6

**[View Project →](https://github.com/KeyurWarkhedkar/mpl)**

---

#### 3. Healio — Smart Appointment & Counselling Platform

Healio is a full-stack healthcare counseling platform built to streamline appointment scheduling and communication between students and counselors.
Developed with Spring Boot, RabbitMQ, Redis, and JWT-based authentication, it offers a secure, scalable, and event-driven backend for real-time and reliable interactions.

🔧 Key Features

🧠 Optimistic Locking & Concurrency Control — Prevents double-booking during simultaneous slot updates.

📬 RabbitMQ for Asynchronous Notifications — Delivers event-based messages like booking confirmations and cancellations without blocking the main workflow.

🔐 JWT & OAuth2 Authentication — Secure login system with Google OAuth integration and stateless session handling.

⚡ Redis Integration — Used for temporary code storage and caching for faster authentication flows.

🗂️ Role-Based Access — Separate dashboards and permissions for counselors and students.

📊 Swagger API Docs — Enables easy API testing and collaboration.

**Tech Stack:** Spring Boot | RabbitMQ | MySQL | Redis | Docker | JWT

**[View Project →](https://github.com/KeyurWarkhedkar/healio)**

---

#### 4. E-Commerce Backend API
🛒 ShopSphere — E-Commerce REST API
A production-grade backend demonstrating robust authentication, complex ORM mappings, and search with dynamic filtering, built as a foundational project in scalable API design.

⚙️ Technical Highlights:

🔐 JWT-Based Authentication & Role-Based Access Control (RBAC) for secure login and authorization

⚙️ Custom Exception Handling ensuring clean and consistent API error responses

🧩 Complex Hibernate Mappings — One-to-Many, Many-to-Many, and cascading relationships across entities

🔍 Dynamic Search with Criteria API supporting filters, pagination, and sorting

🛍️ Cart & Order Management Modules with validation and transactional integrity

📘 RESTful Design with Layered Architecture for maintainability and scalability

**Tech Stack:** Spring Boot | JWT | MySQL | Docker | 

**[View Project →](https://github.com/KeyurWarkhedkar/E-Commerce-Backend-Rest-Api)**

---

# 📊 Problem Solving

**300+ DSA problems solved** across competitive programming platforms

Strong foundation in algorithms, data structures, and optimization techniques

Visit my LeetCode profile: 

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

💡 **Open to backend development opportunities** | Building production-grade concurrent systems
