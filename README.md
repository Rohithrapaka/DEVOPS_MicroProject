# DevOps Micro Project

## Continuous Delivery of a Java Web Application

This project demonstrates a Continuous Integration and Continuous Delivery (CI/CD) pipeline for a Java web application using Spring Boot and GitHub Actions.

## Technologies Used

- Java
- Spring Boot
- Maven
- Git
- GitHub
- GitHub Actions
- Docker

## Project Workflow

Developer pushes code → GitHub repository → GitHub Actions triggers pipeline → Application builds automatically → JAR artifact generated → Docker image built.

## CI/CD Pipeline Steps

1. Checkout repository
2. Setup Java environment
3. Build application using Maven
4. Upload build artifact
5. Build Docker container image

## Application Endpoint

http://localhost:8080

Output:

Continuous Delivery Java App Running!

## Benefits

- Automated build process
- Faster software delivery
- Reduced manual errors
- Containerized deployment