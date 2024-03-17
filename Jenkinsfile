pipeline {
    agent any
    
    stages {
        stage('Build and Push Nextjs Docker Image') {
            steps {
                // Checkout the source code from the repository
                checkout scm
                
                // Build the Docker image for the Go application
                sh 'docker build -t myapp-nextjs .'
            }
        }
    }
}
