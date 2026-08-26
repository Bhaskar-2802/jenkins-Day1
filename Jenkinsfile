pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello from Jenkins - Day 2!'
            }
        }

        stage('Build') {
            steps {
                bat 'echo Building application on Windows'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing application...'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
            }
        }

        stage('Verify') {
            steps {
                echo 'Verifying deployment...'
            }
        }
    }
}