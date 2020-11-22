pipeline {
    agent {
        docker {
            image 'node:latest' 
            args '-p 3000:3000' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                {
                    sh 'sudo chown -R 126:133 "/.npm'
                }
                {
                    sh 'npm install' 
                }
            }
        }
    }
}