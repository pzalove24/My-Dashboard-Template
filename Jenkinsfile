pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Client Test') {
            steps {
                dir('client') {
                    sh 'npm install'
                }
            }
        }
    }
}