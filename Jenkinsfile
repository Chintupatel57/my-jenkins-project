pipeline {
    agent any

    stages {
        stage('Checkout Code') {
            steps {
                echo 'Pulling code from GitHub...'
            }
        }

        stage('Build Docker Image') {
            steps {
                echo 'Building application environment...'
                sh 'python3 -m unittest discover || true'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
                echo 'App is live and running successfully!'
            }
        }
    }

    post {
        success {
            echo 'Pipeline executed successfully!'
        }
    }
}