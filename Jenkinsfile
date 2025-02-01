pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                git branch: 'main', url: 'https://github.com/GnanendharReddy8/Jenkins.git'
            }
        }

        stage('Build') {
            steps {
                sh 'chmod +x HelloWorld.py'
                sh './HelloWorld.py'
            }
        }

        stage('Test') {
            steps {
                sh 'echo "Running tests..."'
            }
        }

        stage('Deploy') {
            steps {
                sh 'echo "Deploying application..."'
            }
        }
    }
}

