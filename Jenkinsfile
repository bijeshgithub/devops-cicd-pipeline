pipeline {
    agent any

    stages {

        stage('Clone Repo') {
            steps {
                git 'https://github.com/bijeshgithub/devops-cicd-pipeline.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t devops-pipeline .'
            }
        }

        stage('List Images') {
            steps {
                sh 'docker images'
            }
        }

    }
}