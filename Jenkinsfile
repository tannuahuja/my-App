pipeline {
    agent any
    
    stages {
        stage('Build and Push WordPress Docker Image') {
            steps {
                // Checkout the source code from the repository
                checkout scm
                
                // Change directory to the 'wordpress' folder
                dir('wordpress') {
                    // Build the Docker image for WordPress
                    sh 'docker build -t my-wordpress .'
                    
                    // Push the Docker image to Docker Hub or another registry
                    sh 'docker push my-wordpress'
                }
            }
        }
    }
}
