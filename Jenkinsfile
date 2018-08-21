pipeline {
  agent {
    docker {
      image 'node:6-alpine'
      args '-p 3003:3003'
    }
    
  }
  stages {
    stage('Build') {
      steps {
        sh 'npm install'
      }
    }
    stage('Test') {
      steps {
        input 'Finished using the web site? (Click "Proceed" to continue)'
      }
    }
    stage('Deliver') {
      steps {
        input 'Finished using the web site? (Click "Proceed" to continue)'
      }
    }
  }
  environment {
    CI = 'true'
  }
}