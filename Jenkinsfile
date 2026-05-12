pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                bat 'echo Building Application...'
            }
        }

        stage('Test') {
            steps {
                bat 'echo Running Tests...'
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
