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
  }
}