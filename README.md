<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=27&duration=2600&pause=900&color=58A6FF&center=true&vCenter=true&width=850&lines=%24+whoami;%3E+Piyush+Prajapati;%3E+Java+Developer+%7C+Backend+Engineering;%3E+Turning+business+workflows+into+backend+systems." alt="Typing introduction" />

<br/>

### Java Developer · Software Development

<sub>I build backend applications where APIs, security, business rules, and data have to work together.</sub>

<br/><br/>

<a href="https://www.linkedin.com/in/piyush-prajapati-22p26/">
  <img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" />
</a>
<a href="mailto:piyushprajapati123piyush@gmail.com">
  <img src="https://img.shields.io/badge/Email-Let's_Talk-EA4335?style=for-the-badge&logo=gmail&logoColor=white" />
</a>
<a href="https://leetcode.com/u/Piyush-2022/">
  <img src="https://img.shields.io/badge/LeetCode-Profile-FFA116?style=for-the-badge&logo=leetcode&logoColor=black" />
</a>

<br/><br/>

<img src="https://komarev.com/ghpvc/?username=prajapatpiyush&label=PROFILE+VIEWS&style=flat-square" alt="Profile views" />

</div>

---

## `$ whoami`

```java
public final class PiyushPrajapati {

    private final String role = "Java Developer";
    private final String focus = "Software Developer";

    private final String[] stack = {
        "Java",
        "Spring Boot",
        "REST APIs",
        "Spring Security",
        "Spring Data JPA",
        "MySQL"
    };

    private final String mindset =
        "Understand the workflow. Model the data. Secure the API. Debug reality.";

    public String currentMission() {
        return "Build backend systems beyond tutorial CRUD";
    }
}
```

I'm a **Computer Science graduate from Indore, India**, focused on building backend and full-stack applications with **Java and Spring Boot**.

What interests me most is not creating another endpoint that performs:

```text
POST → INSERT → 200 OK
```

I prefer working on operations where one request changes the state of an entire workflow:

```text
REQUEST
   │
   ▼
AUTHENTICATION
   │
   ▼
VALIDATION
   │
   ▼
BUSINESS RULES
   │
   ▼
STATE CHANGES
   │
   ▼
PERSISTENCE
   │
   ▼
STRUCTURED RESPONSE
```

**That is the part of backend development I enjoy — understanding what one operation changes across the system.**

---

## `$ ./projects --featured`

### `01` ♻️ EcoTrack

> **A waste submission is not just a database insert.**

A multi-role smart waste management platform connecting **Citizens, Companies, Admins, and recycling operations**.

`Spring Boot` `Spring Security` `JWT` `JPA` `MySQL` `React`

```text
WASTE SUBMITTED
       │
       ├──► Calculate monetary reward
       ├──► Calculate eco-points
       ├──► Update wallet
       ├──► Create CREDIT transaction
       └──► Update waste inventory
                          │
                          ▼
                    CREATE BATCH
                          │
                          ▼
                    ASSIGN RECYCLER
```

**System snapshot**

```text
03 USER ROLES
17 REST CONTROLLERS
14 SERVICE COMPONENTS
26 REACT PAGES
27 APPLICATION ROUTES
```

**Built around**

* Reward and eco-point calculation
* Wallet and transaction tracking
* Waste inventory management
* Batch creation and recycler assignment
* Pickup lifecycle workflows
* JWT authentication and role-based authorization
* Company bulk pickup workflows
* Events, campaigns, and participant management

<a href="https://github.com/prajapatpiyush/EcoTrack-Final">
  <img src="https://img.shields.io/badge/EXPLORE_ECOTRACK-238636?style=for-the-badge&logo=github&logoColor=white" />
</a>

---

### `02` 🛒 E-Commerce Platform

> **The application worked locally. Deployment exposed a bad assumption.**

A full-stack e-commerce management system built with a secured Spring Boot backend.

`Java 17` `Spring Boot` `Spring Security` `JWT` `JPA` `MySQL` `Swagger`

The original image workflow used `MultipartFile` and local storage.

```text
MultipartFile
      │
      ▼
LOCAL /uploads
      │
      ▼
WORKS LOCALLY ✓
      │
      ▼
DEPLOY TO CLOUD
      │
      ▼
INSTANCE RESTARTS
      │
      ▼
IMAGES DISAPPEAR ✗
```

The upload API was not the real problem.

**The storage assumption was.**

I redesigned the image workflow:

```text
                 IMAGE
                   │
          ┌────────┴────────┐
          │                 │
          ▼                 ▼
   UPLOADED FILE      EXTERNAL URL
          │                 │
          └────────┬────────┘
                   │
                   ▼
            SMART RENDERING
```

Then long external image URLs exposed another issue:

```text
VARCHAR(255)
     │
     ▼
DATA TRUNCATION
     │
     ▼
TEXT
```

**Also implemented**

`JWT Authentication` · `Role Authorization` · `DTO Pattern`

`Bean Validation` · `Global Exception Handling`

`Pagination` · `Sorting` · `Swagger` · `Order Analytics`

<a href="https://ecommerce-fullstack-dz04.onrender.com">
  <img src="https://img.shields.io/badge/LIVE_APPLICATION-00C7B7?style=for-the-badge&logo=render&logoColor=white" />
</a>
<a href="https://github.com/prajapatpiyush/ecommerce-fullstack">
  <img src="https://img.shields.io/badge/VIEW_SOURCE-181717?style=for-the-badge&logo=github&logoColor=white" />
</a>

---

### `03` 🎨 PixelCraft Studio

> **Before using Spring abstractions, I built the Java web workflow manually.**

A database-driven Java MVC application with an admin system for managing projects, clients, contact submissions, subscribers, and dynamic website content.

`Java` `JSP` `Servlets` `JDBC` `MySQL` `MVC`

```text
BROWSER
   │
   ▼
SERVLET
   │
   ▼
DAO
   │
   ▼
JDBC
   │
   ▼
MYSQL
   │
   ▼
MODEL
   │
   ▼
JSP
   │
   ▼
DYNAMIC HTML
```

This project gave me the context to understand **why Spring MVC, repositories, ORM, and framework abstractions exist**.

<a href="https://github.com/prajapatpiyush/PixelCraft-Studio-Full-Stack-Java-Web-Application">
  <img src="https://img.shields.io/badge/EXPLORE_PIXELCRAFT-181717?style=for-the-badge&logo=github&logoColor=white" />
</a>

---

## `$ git log --oneline backend-journey`

```text
a91f02c  deployment exposed my assumptions
81bc742  secured APIs with spring-security + jwt
76a10de  started designing REST APIs
61f04ad  moved from JDBC to JPA
52c39ba  understood MVC through implementation
31e87af  learned servlet request-response flow
18b29ce  wrote database operations with DAO + JDBC
0a721df  started with core-java
```

```text
CORE JAVA
    │
    ▼
JDBC + MYSQL
    │
    ▼
DAO + MVC
    │
    ▼
JSP + SERVLETS
    │
    ▼
SPRING BOOT
    │
    ▼
REST APIs + JPA
    │
    ▼
SPRING SECURITY + JWT
    │
    ▼
DEPLOYMENT + DEBUGGING
```

**I prefer understanding why an abstraction exists before depending completely on it.**

---

## `$ cat stack.yml`

<div align="center">

<img src="https://skillicons.dev/icons?i=java,spring,mysql,maven,react,js,html,css,git,github,postman,idea&theme=dark" alt="Technology stack" />

</div>

<br/>

```yaml
backend:
  language: Java
  framework: Spring Boot
  api: REST
  security: Spring Security + JWT
  persistence: Spring Data JPA + Hibernate

database:
  primary: MySQL
  also_used:
    - H2
    - JDBC

architecture:
  - Layered Architecture
  - MVC
  - DAO Pattern
  - DTO Pattern

frontend:
  - React
  - JavaScript
  - HTML5
  - CSS3
  - JSP

currently_improving:
  - Data Structures & Algorithms
  - Backend Design
  - Testing
  - Clean Java
```

## `$ cat current-status.txt`

```text
[ BUILDING ] Stronger Java backend fundamentals
[ SOLVING  ] Data Structures & Algorithms
[ LEARNING ] Backend design and application testing
[ SEEKING  ] Java Developer / Java Backend Developer opportunities
```

🥉 **3rd Prize — National-Level Web Design Competition, Tech-o-tsav**

💼 **Web Developer Intern — Flying Birds Adventure**

🎓 **B.Tech in Computer Science — 2026**

📍 **India**

---

<div align="center">

## `One request. Multiple state changes. One system to keep consistent.`

<br/>

### I don't want my GitHub to say I know Java.

### **I want the repositories to prove it.**

<br/>

<a href="https://www.linkedin.com/in/piyush-prajapati-22p26/">
  <img src="https://img.shields.io/badge/LET'S_CONNECT-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" />
</a>
<a href="https://github.com/prajapatpiyush?tab=repositories">
  <img src="https://img.shields.io/badge/EXPLORE_MY_WORK-181717?style=for-the-badge&logo=github&logoColor=white" />
</a>

<br/><br/>

<code>BUILD → BREAK → DEBUG → UNDERSTAND → REBUILD</code>

</div>
