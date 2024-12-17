# DevOps Basic Application

This repository contains an application demonstrating DevOps fundamentals using different programming languages (Java, Node.js, and Python) along with build and packaging tools. It serves as a foundation for understanding DevOps practices like CI/CD, build automation, and dependency management.

## Technologies Used
- **Java**: Application development using Java with Maven/Gradle for builds.
- **Node.js**: JavaScript runtime for backend services.
- **Python**: Scripts and simple backend examples.
- **DevOps Tools**: Focus on build automation and dependency management.

## Setup Instructions
Follow these steps to set up and run the applications.

### Prerequisites
Ensure you have the following tools installed:
1. **Java Development Kit (JDK)** - [Download JDK](https://adoptopenjdk.net/)
2. **Maven** or **Gradle** (Java Build Tools) - [Download Maven](https://maven.apache.org/)
3. **Node.js** (v14 or later) - [Download Node.js](https://nodejs.org/)
4. **Python** (v3.x) - [Download Python](https://python.org)

Verify the installations:
```bash
java -version
mvn -version
node -v
npm -v
python --version
```

## Building and Running the Application

### Java Application
Navigate to the `java-app` directory:
```bash
cd java-app
```
1. **Build the application** (Maven example):
   ```bash
   mvn clean install
   ```
2. **Run the application**:
   ```bash
   java -jar target/devops-basic-java.jar
   ```

### Node.js Application
Navigate to the `node-app` directory:
```bash
cd node-app
```
1. **Install dependencies**:
   ```bash
   npm install
   ```
2. **Run the application**:
   ```bash
   node index.js
   ```

### Python Application
Navigate to the `python-app` directory:
```bash
cd python-app
```
1. **Run the Python script**:
   ```bash
   python app.py
   ```

---
