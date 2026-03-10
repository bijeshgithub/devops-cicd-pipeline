pipeline {
    agent any

    stages {

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t devops-cicd-pipeline .'
            }
        }

        stage('List out all Docker Images') {
            steps {
                sh 'docker images'
            }
        }

    }
}
