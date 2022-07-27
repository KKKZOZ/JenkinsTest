pipeline {
  agent any
  stages {
    stage('Hello') {
      steps {
        sh 'echo "Hello! This is KKKZOZ speaking!"'
        sh 'echo "This is also KKKZOZ speaking!"'
      }
    }

    stage('Test Docker') {
      steps {
        sh 'docker ps'
      }
    }

    stage('Test MVNW') {
      steps {
        sh 'mvnw clean package'
      }
    }

  }
}