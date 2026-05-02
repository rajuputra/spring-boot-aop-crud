# Enterprise Employee Directory - Spring Boot MVC & AOP

A robust, enterprise-ready CRUD (Create, Read, Update, Delete) web application built with **Spring Boot** and **Spring MVC**. This project demonstrates clean architecture and the practical application of **Aspect-Oriented Programming (AOP)** to handle cross-cutting concerns such as logging across the Controller, Service, and DAO layers.

## 🚀 Features

* **Full CRUD Functionality:** Manage employee data efficiently (Add, Edit, View, Delete).
* **Aspect-Oriented Programming (AOP):** Centralized logging mechanism using `@Aspect`, utilizing `@Before` and `@AfterReturning` advice to track method execution flows without cluttering business logic.
* **Layered Architecture:** Clear separation of concerns utilizing Controller, Service, and DAO (Data Access Object) layers.
* **Modern & Responsive UI:** Server-side rendering with **Thymeleaf**, styled dynamically using **Bootstrap 5** and **Bootstrap Icons** for a clean, professional user experience.

## 🛠️ Tech Stack

* **Backend:** Java, Spring Boot, Spring MVC, Spring AOP
* **Frontend:** Thymeleaf, HTML5, CSS3, Bootstrap 5
* **Database:** MySQL / H2 Database *(Update this based on your actual DB)*
* **Build Tool:** Maven / Gradle *(Update this based on your build tool)*

## 🧠 Technical Highlights: Spring AOP Implementation

Instead of manually adding logging statements inside every method, this project utilizes Spring AOP to automatically intercept method calls. 

**Logging Aspect (`@Aspect`):**
* **Pointcut Declarations:** Intercepts execution across all layers:
  * `execution(* com.yourpackage.controller.*.*(..))`
  * `execution(* com.yourpackage.service.*.*(..))`
  * `execution(* com.yourpackage.dao.*.*(..))`
* **`@Before` Advice:** Logs the method signature and arguments *before* the method executes.
* **`@AfterReturning` Advice:** Logs the method signature and the data returned *after* successful execution.

## 💻 Getting Started

### Prerequisites
* Java 17 or higher
* Maven 3.x
* MySQL Server (if using MySQL)

## ⚙️ Cara Menjalankan Project (Local Development)

1. **Clone repository ini:**
   ```bash
   git clone [https://github.com/username-kamu/nama-repo-kamu.git](https://github.com/username-kamu/nama-repo-kamu.git)

2. **Buka project di IDE (IntelliJ IDEA, Eclipse, atau VS Code).**

3. **Run Script SQL**

4. **Konfigurasi Database:**
Buka file src/main/resources/application.properties dan sesuaikan kredensial database kamu. Contoh untuk MySQL:
Set Properties
   ```bash
   spring.datasource.url=jdbc:mysql://localhost:3306/[nama_database]?useSSL=false&serverTimezone=UTC
   spring.datasource.username=[username_kamu]
   spring.datasource.password=[password_kamu]
   ```
6. **Jalankan Aplikasi:**
Jalankan class utama CruddemoApplication.java.

7. **Akses via Browser:**
Buka http://localhost:8080 di browser Anda.

## 👨‍💻 Penulis
Raju Putra Dermawan Software Engineer | Backend Developer

💼 LinkedIn: [linkedin.com/in/raju-putra-dermawan](https://www.linkedin.com/in/raju-putra-dermawan-244919220/)
