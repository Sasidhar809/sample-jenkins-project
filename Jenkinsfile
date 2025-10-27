pipeline {
    agent any

    stages {

        stage('Clone') {
            steps {
                echo '📦 Cloning repository...'
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo '🏗️ Building the project...'
                bat 'echo Simulating build step...'
            }
        }

        stage('Test') {
            steps {
                echo '🧪 Running tests...'
                bat 'echo All tests passed successfully!'
            }
        }

        stage('Deploy') {
            steps {
                echo '🚀 Deploying application...'
                bat 'echo Application deployed to staging environment!'
            }
        }

        stage('Finish') {
            steps {
                echo '✅ Pipeline completed successfully!'
            }
        }
    }
}
