pipeline {
    agent {
        docker {
            image 'node:15.5.1' 
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