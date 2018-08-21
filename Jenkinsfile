pipeline {
    agent {
        docker {
            image 'node:6-alpine'
            args '-p 3003:3003'
        }
    }
    environment {
        CI = 'true'
    }
    stages {
        stage('Build') {
            steps {
                sh 'npm install'
            }
        }
        stage('Test') {
            steps {
               input message: 'Finished using the web site? (Click "Proceed" to continue)'
            }
        }
        stage('Deliver') {
            steps {
                input message: 'Finished using the web site? (Click "Proceed" to continue)'
            }
        }
    }
}
