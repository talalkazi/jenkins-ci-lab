
pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Checking out GitHub repository'
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo 'Build started'
                sh 'echo "Building project successfully"'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing project'
                sh 'test -f Jenkinsfile'
                sh 'echo "All tests passed"'
            }
        }

        stage('Notify') {
            steps {
                echo 'SUCCESS: CI Pipeline completed!'
            }
        }
    }
}
