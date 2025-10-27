pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                echo 'Cloning repository...'
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo 'Running build stage...'
                bat 'echo Hello from Jenkins running on Windows!'
            }
        }

        stage('Finish') {
            steps {
                echo '✅ Pipeline finished successfully!'
            }
        }
    }
}
