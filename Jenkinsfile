pipeline {
    agent {
        docker {
            image 'node:https://hub.docker.com/_/node/' 
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