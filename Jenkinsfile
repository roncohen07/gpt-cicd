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
                sh 'echo "Deploying application"'
                sh 'ssh sela@146.148.17.73 "cd gpt-cicd && git pull"'
            }
        }
    }
}
