pipeline {
  agent any
  tools {
          maven 'Maven-3.8.6'
          jdk 'JDK17'
      }
  stages {
    stage('Init') {
      steps {
        sh 'echo "Hello! This is KKKZOZ speaking!"'
        sh 'chmod 777 ./mvnw'
        sh 'java --version'
        sh 'mvn -v'
      }
    }

    stage('Test') {
      steps {
        sh 'mvn test'
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
        sh 'mvn clean package'
      }
    }

    stage('Store') {
      steps {
        archiveArtifacts 'target/*.jar'
      }
    }

  }
}