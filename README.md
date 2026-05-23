# 💼 Job Portal — Spring Boot REST API

A production-structured Job Portal backend built with **Spring Boot**, following clean layered architecture (Controller → Service → Repository → Model). Supports full CRUD operations for job postings via RESTful endpoints.

---

## 🚀 Tech Stack

| Layer | Technology |
|---|---|
| Language | Java 17+ |
| Framework | Spring Boot |
| Persistence | Spring Data JPA |
| Database | (H2 / PostgreSQL — configurable) |
| Build Tool | Maven (with Maven Wrapper) |
| Server | Embedded Tomcat |

---

## 🏗️ Project Structure

```
spring-boot-rest/
├── src/
│   └── main/
│       ├── java/
│       │   └── org.example.springbootrest/
│       │       ├── Configuration/      # App-level config (CORS, beans, etc.)
│       │       ├── controller/         # REST controllers (request handling)
│       │       ├── model/              # Entity / data models
│       │       ├── repo/               # Spring Data JPA repositories
│       │       ├── service/            # Business logic layer
│       │       └── SpringBootRestApplication.java
│       └── resources/
│           └── application.properties
├── .gitignore
├── mvnw / mvnw.cmd                     # Maven wrapper scripts
└── pom.xml
```

---

## ✨ Features

- 📋 **View all job postings** — GET all jobs stored in the database
- ➕ **Add new job posts** — POST endpoint with structured job data
- 🔍 **Fetch job by ID** — GET a specific job posting
- ✏️ **Update job details** — PUT endpoint for modifying existing posts
- 🗑️ **Delete a job post** — DELETE endpoint
- ⚙️ **Clean MVC separation** — Controller, Service, Repository, Model layers
- 🔧 **Configuration layer** — Centralized app configuration support

---

## 📦 Getting Started

### Prerequisites
- Java 17+
- Maven (or use the included `mvnw` wrapper)

### Run Locally

```bash
# Clone the repository
git clone https://github.com/your-username/job-portal-spring-boot.git
cd job-portal-spring-boot/spring-boot-rest

# Run using Maven wrapper
./mvnw spring-boot:run
# On Windows:
mvnw.cmd spring-boot:run
```

The server starts at **`http://localhost:8080`**

---

## 🔌 API Endpoints

| Method | Endpoint | Description |
|---|---|---|
| GET | `/jobPosts` | Fetch all job postings |
| GET | `/jobPost/{id}` | Fetch job by ID |
| POST | `/jobPost` | Add a new job posting |
| PUT | `/jobPost` | Update an existing job post |
| DELETE | `/jobPost/{id}` | Delete a job post |

### Sample Job Post JSON

```json
{
  "postId": 1,
  "postProfile": "Java Developer",
  "postDesc": "Looking for a core Java developer with Spring Boot experience",
  "reqExperience": 3,
  "postTechStack": ["Java", "Spring Boot", "REST APIs"]
}
```

---

## 🧠 What I Learned

- Structuring a Spring Boot project with clean layered architecture
- Writing REST controllers and mapping HTTP methods
- Using Spring Data JPA for database operations via Repository pattern
- Configuring Spring Boot with `application.properties`
- Using Maven Wrapper for portable builds

---

## 👤 Author

**Rupam Agrawal**
- GitHub: [@your-username](https://github.com/your-username)
- LinkedIn: [linkedin.com/in/your-profile](https://linkedin.com/in/your-profile)
- Email: rupamagrawal1806@gmail.com

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
