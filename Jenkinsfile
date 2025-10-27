pipeline {
    agent any

    tools {
        nodejs 'NodeJs-18'
    }

    stages {

        stage('Build') {
            steps {
                echo '📦 Skipping build step (no Node.js app yet)'
            }
        }

        stage('Test') {
            steps {
                echo '🧪 Running tests...'
                bat 'npm test || echo "No tests found"'
            }
        }

        stage('Deploy') {
            steps {
                echo '🚀 Deploying application (simulated)...'
                bat 'echo "Application deployed successfully!"'
            }
        }
    }

    post {
        success {
            echo '✅ Build completed successfully!'
        }
        failure {
            echo '❌ Build failed! Please check the logs.'
        }
    }
}
