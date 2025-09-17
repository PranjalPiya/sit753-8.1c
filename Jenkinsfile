pipeline {
  agent any
  stages {
    stage('1. Build') {
      steps { echo 'Task: compile/package | Tools: Maven / Gradle / npm' }
    }
    stage('2. Unit & Integration Tests') {
      steps { echo 'Task: run unit+integration tests | Tools: JUnit / Jest / pytest' }
    }
    stage('3. Code Analysis') {
      steps { echo 'Task: static analysis | Tools: ESLint / Checkstyle / SpotBugs' }
    }
    stage('4. Security Scan') {
      steps { echo 'Task: dependency & vuln scan | Tools: npm audit / OWASP DepCheck / Snyk' }
    }
    stage('5. Deploy to Staging') {
      steps { echo 'Task: ship to staging | Tools: Docker / K8s / Ansible' }
    }
    stage('6. Tests on Staging') {
      steps { echo 'Task: E2E/API tests | Tools: Newman (Postman) / Cypress / Selenium' }
    }
    stage('7. Deploy to Production') {
      steps { echo 'Task: promote to prod (with approval) | Tools: Docker / K8s / Ansible' }
    }
  }
}

// comment for testing