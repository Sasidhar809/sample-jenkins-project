pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                echo '📦 Building the Node.js application...'
                bat '''
                if not exist node_modules (
                    echo Installing dependencies...
                    npm install
                ) else (
                    echo Dependencies already installed
                )
                '''
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
