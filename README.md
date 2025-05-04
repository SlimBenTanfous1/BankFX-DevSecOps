# BankFX – JavaFX Banking App with DevSecOps CI/CD Pipeline

**BankFX** is a simulated desktop banking application built with **JavaFX** that showcases **modern DevSecOps practices**. It includes user authentication, user management (CRUD), and real-time financial data like **stock market trends** and **currency exchange rates** using public APIs.

## Features

- **Login & Sign-Up Interface** with validation
- **User CRUD Management** (Create, Read, Update, Delete)
- **Real-Time Stock & Currency Data** from public APIs
- **Responsive JavaFX GUI**
- **Password Hashing** for secure credentials
- **Containerized with Docker**
- **CI/CD Pipeline using GitHub Actions**
- **Security Scanning Tools Integrated**:
  - Static code analysis (SpotBugs)
  - Dependency scanning (OWASP Dependency-Check)
  - Secrets detection (Gitleaks)

## Project Architecture

[ JavaFX GUI ] --> [ App Logic (Java) ] --> [ SQLite DB or JSON ] --> [ Public API Calls (Stock/Currency) ]


## DevSecOps Pipeline

- **CI/CD** with GitHub Actions:
  - Build and test the app
  - Run security scans (SAST, dependency checks)
  - Package as Docker image

- **Security Checks**:
  - OWASP Dependency-Check: identifies known vulnerable libraries
  - Gitleaks: detects hardcoded secrets
  - SpotBugs: scans for Java code vulnerabilities

## Tech Stack

- **Frontend**: JavaFX (FXML, CSS)
- **Backend**: Java
- **Database**: SQLite or JSON (optional)
- **APIs**: ExchangeRate-API, Yahoo Finance, etc.
- **DevOps**: Docker, GitHub Actions
- **Security**: Gitleaks, SpotBugs, OWASP Dependency-Check

## Getting Started

### Prerequisites

- Java 17+
- Maven or Gradle
- Docker (optional)
- Git

### Clone the Repo

git clone https://github.com/yourusername/BankFX-DevSecOps.git
cd BankFX-DevSecOps

### Build the App
./gradlew build
# or
mvn clean package

### Run the App
java -jar target/BankFX.jar

### Run with Docker
docker build -t bankfx
docker run -it bankfx

### Roadmap
 Basic JavaFX login and registration

 User CRUD operations

 Live stock and currency data

 Docker support

 GitHub Actions pipeline

 Security tools integration

 Kubernetes deployment (future)

 Terraform provisioning for cloud infra (future)


 Created with passion for DevOps + Cybersecurity.
If you like this project, give it a star and share it!
