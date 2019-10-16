pipeline {
  agent any
  stages {
    stage('prova') {
      agent {
        docker {
          image 'node:8'
        }

      }
      steps {
        sh 'npm install'
      }
    }
    stage('test') {
      agent {
        docker {
          image 'maven:3.6.2-jdk-11'
        }

      }
      steps {
        sh 'mvn --version'
      }
    }
  }
}