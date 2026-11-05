pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Getting source code'
            }
        }

        stage('Build') {
            steps {
                sh 'npm install'
            }
        }

        stage('Test') {
            steps {
                sh 'npm test'
            }
        }

        stage('Docker Build') {
            steps {
                sh 'docker build -t devops-task-1 .'
            }
        }
    }
}
