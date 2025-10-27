pipeline {
    agent any

    environment {
        REPO_URL = 'https://github.com/Sasidhar809/sample-jenkins-project.git'
    }

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: "${REPO_URL}", credentialsId: 'YOUR_GITHUB_CREDENTIAL_ID'
            }
        }

        stage('Build') {
            steps {
                echo 'Building the application...'
                bat 'echo Build step executed!'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                bat 'echo Test step executed!'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
                bat 'echo Deploy step executed!'
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully!'
        }
        failure {
            echo 'Pipeline failed!'
        }
    }
}
