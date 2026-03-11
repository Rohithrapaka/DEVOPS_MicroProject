# Continuous Delivery of a Java Web Application

## Project Overview

This project demonstrates the implementation of **Continuous Integration and Continuous Delivery (CI/CD)** for a **Java Spring Boot web application** using **GitHub Actions**.
The goal of this project is to automate the build process so that every code change pushed to the repository is automatically compiled and packaged.

The pipeline ensures that the application is always in a **build-ready and deployable state**.

---

## Technologies Used

* **Java 17**
* **Spring Boot**
* **Maven**
* **Git**
* **GitHub**
* **GitHub Actions (CI/CD)**

---

## Project Architecture

Developer writes code
↓
Code pushed to GitHub repository
↓
GitHub Actions CI/CD Pipeline triggers automatically
↓
Java environment is created
↓
Application is built using Maven
↓
Executable JAR file is generated
↓
Build artifact is stored

---

## Project Structure

```
DEVOPS_MicroProject
│
├── src
│   └── main
│       └── java
│           └── controller
│
├── .github
│   └── workflows
│       └── pipeline.yml
│
├── target
│   └── cd-java-app-0.0.1-SNAPSHOT.jar
│
├── pom.xml
├── mvnw
├── mvnw.cmd
└── README.md
```

---

## Application Functionality

The Spring Boot application exposes a simple REST endpoint.

**Endpoint**

```
http://localhost:8080
```

**Response**

```
Continuous Delivery Java App Running!
```

This confirms that the application is running successfully.

---

## CI/CD Pipeline

The CI/CD pipeline is implemented using **GitHub Actions**.

The pipeline performs the following steps automatically whenever code is pushed to the `main` branch:

1. Checkout repository
2. Install Java environment
3. Build the project using Maven
4. Generate executable JAR file
5. Upload build artifact

Pipeline configuration file:

```
.github/workflows/pipeline.yml
```

---

## How to Run the Application Locally

### 1. Clone the repository

```
git clone https://github.com/Rohithrapaka/DEVOPS_MicroProject.git
```

### 2. Navigate to the project directory

```
cd DEVOPS_MicroProject
```

### 3. Run the application using Maven Wrapper

```
./mvnw spring-boot:run
```

or (Windows)

```
mvnw.cmd spring-boot:run
```

---

### 4. Access the application

Open your browser and go to:

```
http://localhost:8080
```

You should see:

```
Continuous Delivery Java App Running!
```

---

## Build Artifact

After the pipeline runs successfully, Maven generates a **JAR file** inside the `target` directory.

Example:

```
target/cd-java-app-0.0.1-SNAPSHOT.jar
```

This JAR file can be executed using:

```
java -jar target/cd-java-app-0.0.1-SNAPSHOT.jar
```

---

## Learning Outcomes

Through this project, the following DevOps concepts were implemented:

* Continuous Integration
* Continuous Delivery
* Automated build pipelines
* Artifact generation
* GitHub Actions workflow automation

---

## Author

**Rohith Rapaka**

GitHub Repository:
https://github.com/Rohithrapaka/DEVOPS_MicroProject
