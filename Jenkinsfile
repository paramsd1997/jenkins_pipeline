pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                // Define build steps (e.g., invoking Maven, compiling code)
                sh 'echo "buidling steps"'

            }
        }
        stage('Test') {
            steps {
                // Define test steps (e.g., running unit tests)
                sh echo 'mvn test'
            }
        }
        stage('Deploy') {
            steps {
                // Define deployment steps
                sh 'echo "Deployment steps"'
            }
        }
    }
    post {
        success {
            // Actions to perform on success
            echo 'Build successful! Sending notifications...'
        }
        failure {
            // Actions to perform on failure
            echo 'Build failed! Sending notifications...'
        }
    }
}
