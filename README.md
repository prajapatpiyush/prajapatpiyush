
<img
  src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=29&duration=2600&pause=900&color=58A6FF&center=true&vCenter=true&width=950&lines=Piyush+Prajapati;Turning+Workflows+into+Working+Systems.;Building+Beyond+CRUD.;Java+%E2%80%A2+Spring+Boot+%E2%80%A2+Backend+Development"
  alt="Piyush Prajapati animated introduction"
/>

<h3 align="center">Java Developer | Software Developer</h3>

<p align="center">
  <b>Building secure backend systems, REST APIs, and full-stack applications with Java & Spring Boot.</b>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/piyush-prajapati-22p26/">
    <img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
  </a>
  <a href="mailto:piyushprajapati123piyush@gmail.com">
    <img src="https://img.shields.io/badge/Email-Contact_Me-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />
  </a>
  <a href="https://leetcode.com/u/Piyush-2022/">
    <img src="https://img.shields.io/badge/LeetCode-Profile-FFA116?style=for-the-badge&logo=leetcode&logoColor=black" alt="LeetCode" />
  </a>
</p>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=prajapatpiyush&label=Profile%20Views&style=flat-square" alt="Profile Views" />
</p>

---

## 👨‍💻 About Me

I'm a **Computer Science graduate and Java Developer** from India, focused on building backend and full-stack applications using **Java, Spring Boot, REST APIs, Spring Security, and MySQL**.

My projects go beyond basic CRUD. I enjoy working on applications where a single operation can involve **authentication, validation, business rules, multiple database changes, and a complete application workflow**.

* 🔭 Currently building and improving **Java & Spring Boot applications**
* 🌱 Strengthening **Data Structures & Algorithms, backend design, and testing**
* 🔐 Interested in **REST API development, authentication, authorization, and business logic**
* 🧠 Built systems involving **wallets, transactions, inventory, order workflows, analytics, and multi-role access**
* 💼 Open to **Java Developer, Java Backend Developer, and Software Developer opportunities**
* 📍 Based in **India**

---

## 🛠️ Tech Stack

<p align="center">
  <img src="https://skillicons.dev/icons?i=java,spring,mysql,maven,react,js,html,css,git,github,postman,idea,vscode,eclipse&theme=dark" alt="Technology Stack" />
</p>

### Backend Development

`Java` · `Spring Boot` · `Spring MVC` · `Spring Security` · `Spring Data JPA` · `Hibernate`

`REST APIs` · `JWT Authentication` · `JDBC` · `JSP` · `Servlets`

### Database & Persistence

`MySQL` · `H2 Database` · `SQL` · `JPA` · `Hibernate` · `JDBC`

### Frontend Development

`React` · `JavaScript ES6+` · `HTML5` · `CSS3`

### Architecture & Backend Concepts

`Layered Architecture` · `MVC` · `DAO Pattern` · `DTO Pattern`

`Role-Based Authorization` · `Bean Validation` · `Global Exception Handling`

`Pagination` · `Sorting` · `API Documentation`

### Tools

`Git` · `GitHub` · `Postman` · `Swagger / OpenAPI` · `Maven`

`IntelliJ IDEA` · `Spring Tool Suite` · `VS Code` · `Eclipse`

---

# 🚀 Featured Projects

## ♻️ EcoTrack — Smart Waste Management System

> A multi-role waste management platform designed around real operational workflows instead of isolated CRUD operations.

<p>
  <a href="https://github.com/prajapatpiyush/EcoTrack-Final">
    <img src="https://img.shields.io/badge/View_Repository-181717?style=for-the-badge&logo=github&logoColor=white" alt="EcoTrack Repository" />
  </a>
</p>

**Tech Stack:** `Spring Boot` `Spring Security` `JWT` `Spring Data JPA` `MySQL` `React`

### Key Features

* 👥 Multi-role architecture for **Citizen, Company, and Admin**
* 🔐 Stateless authentication using **Spring Security and JWT**
* 💰 Dynamic **waste reward and eco-point calculation engine**
* 👛 Wallet balance and financial transaction tracking
* 📦 Waste inventory management and quantity tracking
* ♻️ Waste batch creation and recycler assignment workflow
* 🚚 Citizen and company pickup scheduling
* 📊 Admin analytics and platform management
* 📢 Environmental campaigns and sustainability blogs
* 📅 Events with participant registration and capacity tracking
* 🌙 Responsive React interface with dark mode support

### System Workflow

```text
Waste Submission
       │
       ├── Calculate Monetary Reward
       ├── Calculate Eco Points
       ├── Update User Wallet
       ├── Create Transaction
       └── Update Waste Inventory
                      │
                      ▼
               Create Waste Batch
                      │
                      ▼
               Assign Recycler
```

### Project Scale

`3 User Roles` · `17 REST Controllers` · `14 Service Components`

`26 React Pages` · `27 Application Routes`

**What I learned:** Designing business workflows where one request affects multiple parts of an application's state while maintaining security and data consistency.

---

## 🛒 Full-Stack E-Commerce Admin Platform

> A secured e-commerce management system with REST APIs, role-based access, product management, order workflows, and analytics.

<p>
  <a href="https://github.com/prajapatpiyush/ecommerce-fullstack">
    <img src="https://img.shields.io/badge/View_Repository-181717?style=for-the-badge&logo=github&logoColor=white" alt="E-Commerce Repository" />
  </a>
  <a href="https://ecommerce-fullstack-dz04.onrender.com">
    <img src="https://img.shields.io/badge/Live_Demo-00C7B7?style=for-the-badge&logo=render&logoColor=white" alt="Live Demo" />
  </a>
</p>

**Tech Stack:** `Java 17` `Spring Boot` `Spring Security` `JWT` `JPA` `MySQL` `Swagger`

### Key Features

* 🔐 JWT authentication and role-based authorization
* 👤 Admin and User access control
* 📦 Product and category management
* 🛍️ Order processing and order item relationships
* 📊 Revenue and order analytics
* 📄 Pagination and dynamic sorting
* ✅ Request validation using Bean Validation
* 🚨 Centralized exception handling using `@ControllerAdvice`
* 📘 REST API documentation with Swagger / OpenAPI
* 🖼️ Hybrid image management supporting uploaded files and external URLs

### A Deployment Problem I Solved

The original application stored uploaded images in a local `/uploads` directory.

It worked locally.

After cloud deployment, instance restarts caused uploaded images to disappear because the application relied on temporary local storage.

```text
Local Development
MultipartFile → /uploads → Image Available ✓

Cloud Deployment
MultipartFile → Temporary Storage → Restart → Image Lost ✗
```

I redesigned the image workflow to support both:

```text
             IMAGE
               │
      ┌────────┴────────┐
      ▼                 ▼
Uploaded File      External URL
      │                 │
      └────────┬────────┘
               ▼
        Dynamic Rendering
```

Long external image URLs later exposed a database column limitation, so the image field was changed from `VARCHAR` to `TEXT`.

**What I learned:** Code working on localhost does not prove that its infrastructure assumptions will survive deployment.

---

## 🎨 PixelCraft Studio — Full Stack Java Web Application

> A database-driven Java MVC application built using JSP, Servlets, JDBC, and MySQL.

<p>
  <a href="https://github.com/prajapatpiyush/PixelCraft-Studio-Full-Stack-Java-Web-Application">
    <img src="https://img.shields.io/badge/View_Repository-181717?style=for-the-badge&logo=github&logoColor=white" alt="PixelCraft Repository" />
  </a>
</p>

**Tech Stack:** `Java` `JSP` `Servlets` `JDBC` `MySQL` `MVC`

### Key Features

* 🧑‍💼 Admin dashboard for content management
* 🎨 Project management
* 👥 Client management
* 📩 Contact form submission tracking
* 📧 Newsletter subscriber management
* 🗄️ MySQL database persistence
* 🔄 Dynamic JSP content rendering
* 🏗️ MVC and DAO-based architecture

### Application Flow

```text
Browser Request
       │
       ▼
Servlet Controller
       │
       ▼
DAO Layer
       │
       ▼
JDBC
       │
       ▼
MySQL
       │
       ▼
Java Model
       │
       ▼
JSP View
       │
       ▼
Dynamic HTML Response
```

**What I learned:** Building the Java web workflow manually helped me understand why Spring MVC, repositories, dependency injection, and ORM abstractions exist.

---

## 📈 My Java Backend Journey

```text
Core Java
    │
    ▼
JDBC + MySQL
    │
    ▼
DAO Pattern
    │
    ▼
JSP + Servlets
    │
    ▼
MVC Architecture
    │
    ▼
Spring Boot
    │
    ▼
Spring Data JPA
    │
    ▼
REST API Development
    │
    ▼
Spring Security + JWT
    │
    ▼
Deployment & Debugging
```

> **I prefer understanding why an abstraction exists before depending completely on it.**

---

## 🎓 Education

**Bachelor of Technology — Computer Science**

Swami Vivekanand College of Engineering, Indore

`2022 – 2026` · `CGPA: 7.26`

---

## 💼 Experience

### Web Developer Intern — Flying Birds Adventure

`June 2025 – September 2025`

* Developed and maintained responsive web interfaces using HTML, CSS, and JavaScript
* Implemented feature enhancements for client projects
* Collaborated on application updates and database-driven workflows

---

## 🏆 Achievement

🥉 **3rd Prize — National-Level Web Design Competition**

Secured 3rd Prize at **Tech-o-tsav**, organized by Acropolis Institute, Indore.

---

## 📜 Certification

🎓 **Full Stack Java Development Certification**

Programming World — Completed

---

## 🎯 Currently Focused On

* ☕ Strengthening Core Java and backend fundamentals
* 🧩 Solving Data Structures & Algorithms problems
* 🏗️ Improving backend application design
* 🧪 Learning application testing practices
* ✨ Writing cleaner and more maintainable Java code

---

## 🌐 Connect With Me

<p align="center">
  <a href="https://github.com/prajapatpiyush">
    <img src="https://img.shields.io/badge/GitHub-prajapatpiyush-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" />
  </a>
  <a href="https://www.linkedin.com/in/piyush-prajapati-22p26/">
    <img src="https://img.shields.io/badge/LinkedIn-Piyush_Prajapati-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
  </a>
  <a href="https://leetcode.com/u/Piyush-2022/">
    <img src="https://img.shields.io/badge/LeetCode-Piyush--2022-FFA116?style=for-the-badge&logo=leetcode&logoColor=black" alt="LeetCode" />
  </a>
</p>

---

<div align="center">

### I don't want my GitHub to just say I know Java.

### **I want my projects to prove it.**

<br/>

<code>BUILD → BREAK → DEBUG → UNDERSTAND → IMPROVE</code>

<br/><br/>

<b>Open to Java Developer · Java Backend Developer · Software Developer opportunities</b>

</div>
