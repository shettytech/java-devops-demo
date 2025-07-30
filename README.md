# Java DevOps CI/CD Demo

This is a simple Java project built with Maven to demonstrate DevOps CI/CD using **GitHub Actions**.

---

##  Project Structure

ava-devops-demo/
├── src/
│ ├── main/java/com/example/App.java
│ └── test/java/com/example/AppTest.java
├── pom.xml
└── .github/workflows/ci.yml


---

## Technologies Used

- Java 17
- Maven
- GitHub Actions
- JUnit 4

---

## Setup Instructions

### 1. Clone the Repository
git clone git@github.com:<your-username>/java-devops-demo.git
cd java-devops-demo

### 2. Build the Project Locally
mvn clean package

### 3. Run Tests Locally
mvn test

### 4. CI/CD with GitHub Actions
This workflow runs on every push to main and performs:

Checkout

Java setup

Maven build

Test execution
### 5. Workflow File: .github/workflows/ci.yml
### 6. Dockerfile
### 7. Build Docker Image
mvn clean package
docker build -t java-devops-demo .
### 8. Run Docker Container
docker run --rm java-devops-demo

### 8. Deploy to AWS Elastic Beanstalk
eb init -p java-17 java-devops-demo
eb create dev-env
eb deploy
