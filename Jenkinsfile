pipeline {
    agent {
        docker {
            image 'node:latest' 
            args '-p 8080:8080'
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'npm install' 
            }
        }
    }
}