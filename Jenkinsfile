pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git 'https://github.com/sasisasi25/simple-web-app.git'
            }
        }

        stage('Build') {
            steps {
                bat 'echo Build Number: %BUILD_NUMBER%'
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
