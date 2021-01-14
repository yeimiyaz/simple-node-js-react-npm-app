pipeline {
    agent {
        docker {
            image 'node:latest' 
            args '-p 3000:3000'
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
				sh "chmod +x -R ${env.WORKSPACE}"
                sh './jenkins/scripts/test.sh'
            }
        }
    }
}