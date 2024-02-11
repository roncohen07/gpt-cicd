pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                // Add commands to build your application
                sh 'echo "Building application"'
            }
        }
        
        stage('Test') {
            steps {
                // Add commands to run tests
                sh 'echo "Running tests"'
            }
        }
        
        stage('Deploy') {
            when {
                branch 'main'
            }   
            steps {
                // Add commands to deploy your application
                // For demonstration, let's assume deploying to a server via SSH
                sh 'echo "Deploying application..."'
                sh 'scp index.html sela@146.148.17.73:/var/www/html'
            }
        }

    }
}
