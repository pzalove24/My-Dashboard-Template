pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Client Test') {
            dir('client') {
                sh 'npm install'
            }
        }
    }
}