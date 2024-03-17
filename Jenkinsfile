pipeline {
    agent any
    
    stages {
        stage('Build and Push Go Docker Image') {
            steps {
                // Checkout the source code from the repository
                checkout scm
                
                // Change directory to the 'go' folder
                dir('go') {
                    // Build the Docker image for the Go application
                    sh 'docker build -t myapp-go .'
                }
            }
        }
    }
}
