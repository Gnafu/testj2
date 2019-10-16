pipeline {
  agent {
    docker {
      image 'node:8'
    }

  }
  stages {
    stage('prova') {
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