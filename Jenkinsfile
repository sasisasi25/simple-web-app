pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git 'https://github.com/USERNAME/simple-web-app.git'
            }
        }

        stage('Build') {
            steps {
                bat 'echo Building Application...'
            }
        }

        stage('Test') {
            steps {
                bat 'echo Testing Application...'
            }
        }

        stage('Deploy') {
            steps {
                bat '''
                xcopy /E /Y * C:\\Deployments\\simple-web-app\\
                '''
            }
        }
    }
}