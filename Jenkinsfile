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

    stage('Content Introspect') {
      steps {
        sh 'ls'
        sh 'chmod 777 ./mvnw'
        sh 'java --version'
      }
    }

    stage('MVNW') {
      steps {
        sh './mvnw clean package'
      }
    }

  }
}