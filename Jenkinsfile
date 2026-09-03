pipeline {
  agent any

  stages {
    stage('1. Build') {
      steps {
        echo 'Stage 1: Build'
        echo 'Build the code using Maven'
      }
    }
    
    stage('2. Unit and Integration Tests') {
      steps {
        echo 'Stage 2: Unit and Integration Tests'
        echo 'Run unit tests using JUnit and TestNG'
      }
    }
    
    stage('3. Code Analysis') {
      steps {
        echo 'Stage 3: Code Analysis'
        echo 'Perform quality check with SonarQube'
      }
    }

    stage('4. Security Scan') {
      steps {
        echo 'Stage 4: Security Scan'
        echo 'Scan dependencies using OWASP Dependency-Check'
      }
    }

    stage('5. Deploy to Staging') {
      steps {
        echo 'Stage 5: Deploy to Staging'
        echo 'Deploy to AWS EC2'
      }
    }

    stage('6. Integration Tests of Staging') {
      steps {
        echo 'Stage 6: Integration Tests of Staging'
        echo 'Run integration tests using Newman'
      }
    }

    stage('7. Deploy to Production') {
      steps {
        echo 'Stage 7: Deploy to Production'
        echo 'Deploy build using AWS EC2'
      }
    }
  }

  post {
    success {
      echo 'Pipeline completed successfully'
    }
    failure {
      echo 'Pipeline failed'
    }
  }
}
                
