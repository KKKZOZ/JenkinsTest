pipeline {
  agent any
  stages {
    stage('Init') {
      steps {
        sh 'echo "Hello! This is KKKZOZ speaking!"'
        sh 'chmod 777 ./mvnw'
      }
    }

    stage('Test') {
      steps {
        sh './mvnw test'
      }
    }

    stage('Content Introspect') {
      steps {
        sh 'ls'
        sh 'java --version'
      }
    }

    stage('MVNW') {
      steps {
        sh './mvnw clean package'
      }
    }

    stage('Store') {
      steps {
        archiveArtifacts 'target/*.jar'
      }
    }

  }
}