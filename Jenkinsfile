pipeline {
  agent any
  stages {
    stage('Hello') {
      steps {
        sh 'echo "This is also KKKZOZ speaking!"'
        sh 'echo "Hello! This is KKKZOZ speaking!"'
      }
    }

    stage('Test Docker') {
      steps {
        sh 'docker ps'
      }
    }

    stage('Content Introspect') {
      steps {
        sh 'java --version'
        sh 'ls'
        sh 'chmod 777 ./mvnw'
      }
    }

    stage('MVNW') {
      steps {
        sh './mvnw clean package'
      }
    }

  }
}