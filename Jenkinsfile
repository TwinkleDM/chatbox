pipeline {
    agent any
    environment {
        CI = 'true'
    }
    stages {
        stage('Build') {
            steps {
                sh 'npm install'
            }
        }
        stage('Test') {
            steps {
                sh 'npm install'
            }
        }
        stage('Deliver for development') {
            when {
                branch 'development' 
            }
            steps {
                sh 'pwd'
            }
        }
        stage('Deploy for production') {
            when {
                branch 'production'  
            }
            steps {
               sh npm install
            }
        }
    }
}
