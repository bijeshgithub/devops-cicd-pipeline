pipeline {
    agent any

    stages {

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t devops-cicd-pipeline .'
            }
        }

        stage('List Docker Images') {
            steps {
                sh 'docker images'
            }
        }

    }
}
