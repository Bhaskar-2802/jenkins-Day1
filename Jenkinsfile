pipeline {
    agent any

    environment {
        APP_NAME = 'Jenkins-Day3'
        ENVIRONMENT = 'DEV'
    }

    stages {

        stage('Hello') {
            steps {
                echo 'Hello from Jenkins!'
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

        stage('Credentials Test') {
            steps {
                withCredentials([string(credentialsId: 'day3-secret', variable: 'MY_SECRET')]) {
                    bat 'echo Jenkins credential is available'
                }
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

        stage('Environment') {
            steps {
                echo "Application: ${APP_NAME}"
                echo "Environment: ${ENVIRONMENT}"
                echo "Build Number: ${BUILD_NUMBER}"
            }
        }
    }
}