pipeline {
    agent any
    
    stages {
        stage('Build WordPress Docker Image') {
            steps {
                // Checkout the source code from the repository
                checkout scm
                
                // Build the Docker image for WordPress
                sh 'docker build -t my-wordpress .'
            }
        }
    }
}
