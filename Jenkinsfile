pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo '''Stage 1: Build
Task: Compile and package the application.
Tool: Maven'''
      }
    }
    stage('Unit and Integration Tests') {
      steps {
        echo '''Stage 2: Unit and Integration Tests
Task: Run unit tests and integration tests.
Tool: JUnit with Maven Surefire/Failsafe'''
      }
    }
    stage('Code Analysis') {
      steps {
        echo '''Stage 3: Code Analysis
Task: Static code analysis.
Tool: SonarQube Scanner'''
      }
    }
    stage('Security Scan') {
      steps {
        echo '''Stage 4: Security Scan
Task: Scan for vulnerabilities.
Tool: OWASP Dependency-Check'''
      }
    }
    stage('Deploy to Staging') {
      steps {
        echo '''Stage 5: Deploy to Staging
Task: Deploy to a staging server.
Tool: Ansible'''
      }
    }
    stage('Integration Tests on Staging') {
      steps {
        echo '''Stage 6: Integration Tests on Staging
Task: Run integration tests in staging.
Tool: Newman (Postman CLI)'''
      }
    }
    stage('Deploy to Production') {
      steps {
        echo '''Stage 7: Deploy to Production
Task: Deploy to production server.
Tool: Ansible'''
      }
    }
  }
}
