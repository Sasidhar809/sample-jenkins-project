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
                sh 'bash hello.sh'
            }
        }

        stage('Finish') {
            steps {
                echo 'Build completed successfully!'
            }
        }
    }
}
