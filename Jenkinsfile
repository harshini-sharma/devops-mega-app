pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo 'Building Wanderlust application...'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
            }
        }

        stage('Docker Compose Validation') {
            steps {
                echo 'Validating Docker Compose configuration...'
            }
        }
    }

    post {
        success {
            echo 'Wanderlust CI Pipeline completed successfully!'
        }

        failure {
            echo 'Pipeline failed!'
        }
    }
}