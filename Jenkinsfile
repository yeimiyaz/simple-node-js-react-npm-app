pipeline {
    agent {
        docker {
            image 'node:14.15.4-slim' 
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